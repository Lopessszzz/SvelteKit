<!-- Badge.svelte -->

<script>
    export let text = 'Exemplo'; 
    export let color = 'primary'; 
  </script>
  

  <style>
    .badge {
      display: inline-block;
      padding: 0.25em 0.4em;
      font-size: 75%;
      font-weight: 700;
      line-height: 1;
      text-align: center;
      white-space: nowrap;
      vertical-align: baseline;
      border-radius: 0.25rem;
    }
  
    .primary {
      background-color: #007bff;
      color: #fff;
    }
  
    .secondary {
      background-color: #6c757d;
      color: #fff;
    }
  
    .success {
      background-color: #28a745;
      color: #fff;
    }
  
  </style>
  
 
  <span class="badge {color}">{text}</span>