<script lang="ts">
	import { LineChart } from 'layerchart';
	import { curveCatmullRom } from 'd3-shape';
</script>

<div class="flex w-full justify-center py-12">
	<div class="chart-wrapper border">
		<LineChart
			data={[
				{
					date: '2025-02-22',
					value: 0
				},
				{
					date: '2025-02-23',
					value: 0
				},
				{
					date: '2025-02-24',
					value: 0
				},
				{
					date: '2025-02-25',
					value: 0
				},
				{
					date: '2025-02-26',
					value: 0
				},
				{
					date: '2025-02-27',
					value: 0
				},
				{
					date: '2025-02-28',
					value: 3
				}
			]}
			x="date"
			y="value"
			props={{ spline: { curve: curveCatmullRom } }}
			renderContext="svg"
		/>
	</div>
</div>

<style>
	.chart-wrapper {
		width: 100%;
		max-width: 900px;
		height: 300px;
		position: relative;
	}
</style>
