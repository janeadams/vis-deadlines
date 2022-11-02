<script>
    import '../app.scss';
    import Nav from '$lib/Nav.svelte';
    import { CSVDownloader } from 'svelte-csv';
  </script>
  
  <div class="g-app-wrapper">
    <Nav/>
    <slot></slot>
    <CSVDownloader filename={'$../static/data/deadlines.csv'}></CSVDownloader>
  </div>