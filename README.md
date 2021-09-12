
# Svelte DataTables

This project brings DataTable into your Svelte project.

DataTable is a popular JavaScript library allowing you to easily display
your data in a user-friendly table.   

You can find more information about DataTable on : https://www.datatables.net




Installation
------------

To install it, you will need to run :

    //install with npm
    npm install svelte-advanced-tables 
    //install with yarn or others
    yarn : yarn add svelte-advanced-tables




Getting started
---------------

After installing it, to use it, follow the steps below:

    import Table from 'svelte-advanced-tables'
    
    let data = {
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
    };
    
    //Call the component into your svelte page
    
    <Table /> //When no data are provided, it loads some default data
    
    <Table table_data="{data}" /> //Here is the way to add custom data
  

## Examples

You will it find in the folder : [sample](https://github.com/homescriptone/svelte-datatables/tree/main/sample/)


## Contribution

If you feel that important features are missing, you are free to send a pull request.


## Credits

Maintainer: [Emmanuel ADEKPLOVI](https://github.com/manutheblacker)

⌨️ Build with ❤️ by [HomeScript](https://github.com/homescriptone) 😊

