<script>
    export let tableData = []  ;
    //import the svelte-datatable.css
    //import the svelte-datatable.js
    import 'bootstrap5'
    import {onMount} from 'svelte'
    let all_rows, all_columns;
    onMount(()=>{
      var dataTableEl = document.getElementById('datatable');
      const dataTable = new simpleDatatables.DataTable(dataTableEl);
    });
  </script>
  
  <main>
      <div class="table-responsive py-4">
          <table class="table table-flush" id="datatable">
              <thead class="thead-light">
              <tr>
                  {#each tableData.all_columns  as table_col_name }
                      <th>{table_col_name}</th>
                  {/each}
              </tr>
              </thead>
              <tbody>
              {#each tableData.all_rows as rows }
                  <tr>
                         <td>Your rows data</td>
                  </tr>
              {/each}
              </tbody>
          </table>
      </div>
  </main>
  