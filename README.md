
# Svelte DataTables

This repository bring DataTable into your Svelte or Svelte Frameworks
projects.

Maintainer: [Emmanuel ADEKPLOVI](https://github.com/manutheblacker)

Installation
------------

    npm install homescriptone/svelte-advanced-tables



Getting started
---------------

    import Table from 'svelte-advanced-tables'
    
    let data = [
            'rows' : [
                [
                  'TOTAL',
                  'Djim'
                ]
            ], 
            'columns' : [
                'Entreprise',
                'First Name'
            ],
            'styles'  : [
                'thead' : '',
                'tbody' : ''
            ],
    ];
    
    //Call the component into your svelte page
    
    <Table /> //When no data are provided, it loads some default data
    
    <Table table_data="{data}" /> //Here is the way to add custom data
  
   
## Contribution

Feel free to improve it by sending MR

⌨️ Build with ❤️ by [HomeScript](https://github.com/homescriptone) 😊

