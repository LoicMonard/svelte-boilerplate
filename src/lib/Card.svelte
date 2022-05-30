<script>
  export let card = {}
</script>

<li class="card">
  <h2>{card.title}</h2>
  <p>{card.description}</p>
</li>

<style>
  .card {
    background: #fff;
    border-radius: 4px;
    box-shadow: 0 2px 3px rgba(10, 10, 10, 0.1), 0 0 0 1px rgba(10, 10, 10, 0.1);
    padding: 1em;
    margin: 1em;
  }
</style>
