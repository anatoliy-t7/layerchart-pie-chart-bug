<script lang="ts">
	import { PieChart } from 'layerchart';

	const colors = [
		'oklch(0.645 0.246 16.439)',
		'oklch(0.723 0.219 149.579)',
		'oklch(0.623 0.214 259.815)',
		'oklch(0.769 0.188 70.08)',
		'oklch(0.704 0.14 182.503)',
		'oklch(0.768 0.233 130.85)',
		'oklch(0.667 0.295 322.15)',
		'oklch(0.606 0.25 292.717)',
		'oklch(0.656 0.241 354.308)',
		'oklch(0.795 0.184 86.047)',
		'oklch(0.585 0.233 277.117)',
		'oklch(0.685 0.169 237.323)',
		'oklch(0.705 0.213 47.604)',
		'oklch(0.696 0.17 162.48)',
		'oklch(0.715 0.143 215.221)',
		'oklch(0.627 0.265 303.9)'
	];
</script>

<div class="flex w-full justify-center py-12">
	<div class="chart-wrapper">
		<PieChart
			data={[
				{
					year: 2019,
					basket: 1,
					fruit: 'apples',
					value: 3840
				},
				{
					year: 2019,
					basket: 1,
					fruit: 'bananas',
					value: 1920
				},
				{
					year: 2019,
					basket: 2,
					fruit: 'cherries',
					value: 960
				},
				{
					year: 2019,
					basket: 2,
					fruit: 'grapes',
					value: 400
				}
			]}
			key="fruit"
			value="value"
			cRange={colors}
			innerRadius={-36}
			cornerRadius={5}
			padAngle={0.02}
		/>
	</div>
</div>

<style>
	.chart-wrapper {
		width: 300px;
		height: 300px;
		position: relative;
	}
</style>
