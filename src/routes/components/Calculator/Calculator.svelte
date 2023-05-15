<script>
	import { co2 } from '@tgwf/co2';
	import { onMount } from 'svelte';
    

	const co2Emission = new co2();

	let estimatedCO2 = null;
	let bytesSentMB = ''; // Initial value of bytesSent in megabytes as an empty string
	let bytesSent = 0; // Default value of bytesSent as 0 bytes
	let pageViews = 1; // Default value of page views
	let greenHost = false; // Is the data transferred from a green host?
	let emissionUnit = 'grams'; // Default emission unit: grams or tons

	function calculateCO2() {
		if (bytesSentMB !== '') {
			bytesSent = parseFloat(bytesSentMB) * 1000000; // Convert bytesSent to bytes
		}

		estimatedCO2 = co2Emission.perByte(bytesSent, greenHost);

		if (emissionUnit === 'tons') {
			estimatedCO2 /= 1000000; // Convert grams to tons
		}

		estimatedCO2 *= pageViews; // Multiply by page views
	}

	onMount(() => {
		calculateCO2(); // Calculate initial CO2 emissions on component mount
	});

	function handleBytesSentChange(event) {
		bytesSentMB = event.target.value;
	}

	function handlePageViewsChange(event) {
		const input = event.target.value.replace(/,/g, ''); // Remove commas from the input
		pageViews = parseInt(input, 10);
	}

	function handleEmissionUnitChange(event) {
		emissionUnit = event.target.value;
		calculateCO2(); // Recalculate CO2 emissions when the unit changes
	}
</script>

<div class="calc-navbar">
    <a href="/">Guidelines</a>
</div>

<div class="calc-container">
	<div>
    <h1>Calculate CO2 Emissions</h1>
    <p>
        Data Amount: <input type="text" bind:value={bytesSentMB} on:input={handleBytesSentChange} /> MB
    </p>
    <p>
        Page Views: <input type="text" bind:value={pageViews} on:input={handlePageViewsChange} />
    </p>
    <p>
        <label>
            <input type="radio" bind:group={greenHost} value={false} />
            Data transferred from a non-green host
        </label>
    </p>
    <p>
        <label>
            <input type="radio" bind:group={greenHost} value={true} />
            Data transferred from a green host
        </label>
    </p>
    <p>
        <label>
            <input type="radio" bind:group={emissionUnit} value="grams" />
            CO2 Emissions in grams
        </label>
    </p>
    <p>
        <label>
            <input type="radio" bind:group={emissionUnit} value="tons" />
            CO2 Emissions in tons
        </label>
    </p>
    <p>
        <button on:click={calculateCO2}>Calculate</button>
    </p>
    {#if estimatedCO2 !== null}
        <p>
            Sending {bytesSentMB || '0'} MB of data returns a carbon footprint of {estimatedCO2.toFixed(3)}
            {emissionUnit === 'tons' ? 'tons' : 'grams'} of CO2
        </p>
    {/if}
	</div>
</div>

<style>
	@import './Calculator.css';
</style>