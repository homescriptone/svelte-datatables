
# Svelte DataTables

This repository bring DataTables into your Svelte or Svelte Frameworks
projects.

Maintainer: [Emmanuel ADEKPLOVI](https://github.com/manutheblacker)

Installation
------------

    npm install homescriptone/svelte-datatables



Getting started
---------------

    import Table from 'svelte-datatables'
    
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

