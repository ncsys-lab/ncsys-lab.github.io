<!-- Slots into the "Assignments" column -->

<div>
	<slot />
</div>

<style>
	div {
		grid-area: assignments;
    display: flex;
    flex-wrap: wrap;
	}
</style>