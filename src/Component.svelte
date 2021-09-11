<script>
    export let table_data = {
        'rows' : [
            [
                "Bill", '23', 'day one'
            ],
            [
                "John", '34', 'day two'
            ],
            [
                "Hermann", '45', 'day three'
            ],
            [
                "Femi", '56', 'day four'
            ],
            [
                "Bill", '23', 'day one'
            ],
            [
                "John", '34', 'day two'
            ],
            [
                "Hermann", '45', 'day three'
            ],
            [
                "Femi", '56', 'day four'
            ],
            [
                "Bill", '23', 'day one'
            ],
            [
                "John", '34', 'day two'
            ],
            [
                "Hermann", '45', 'day three'
            ],
            [
                "Femi", '56', 'day four'
            ],
            [
                "Bill", '23', 'day one'
            ],
            [
                "John", '34', 'day two'
            ],
            [
                "Hermann", '45', 'day three'
            ],
            [
                "Femi", '56', 'day four'
            ],
            [
                "Bill", '23', 'day one'
            ],
            [
                "John", '34', 'day two'
            ],
            [
                "Hermann", '45', 'day three'
            ],
            [
                "Femi", '56', 'day four'
            ],
        ],
        'columns' : [
            'Full Name :',
            'Age :',
            'Start working on :'
        ],
        'styles' : [],
    };
    import './assets/datatable.css'
    import simpleDatatables from './assets/datatable.js'

    import {onMount} from 'svelte'
    onMount(()=>{
      var dataTableEl = document.getElementById('datatable');
      new simpleDatatables.DataTable(dataTableEl);
    });
  </script>
  
  <main>
      <div class="table-responsive py-4">
          <table class="table table-flush" id="datatable">
              <thead class="svelte-datatable-thead thead-light {table_data.styles.thead}">
              <tr>
                  {#each table_data.columns  as table_col_name }
                    <th>{table_col_name}</th>
                  {/each}
              </tr>
              </thead>
              <tbody  class="svelte-datatable-tbody {table_data.styles.tbody}">
                {#each table_data.rows as table_rows }
                <tr>
                    {#each table_rows as rows }
                        <td>{rows}</td>
                    {/each}      
                  </tr>
                {/each}
              </tbody>
          </table>
      </div>
  </main>