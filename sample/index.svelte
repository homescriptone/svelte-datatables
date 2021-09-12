<script>
	export let name = "Jorg";
	import Table from 'svelte-advanced-tables'
	let data = {
        'rows' : [
            [
                "Bill", '23', '2021'
            ],
            [
                "John", '34', '2022'
            ],
            [
                "Hermann", '45', '2023'
            ],
        ],
        'columns' : [
            'Full Name :',
            'Age :',
            'Year : '
        ],
    };
</script>

<main>
	<h1> Hello world! {name} </h1>
	<!-- Initialize the table without args -->
	<Table  />
	<!-- Initialize the table with args -->
	<Table table_data ="{data}"  />
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>