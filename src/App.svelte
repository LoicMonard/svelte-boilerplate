<script>
  import Card from './lib/Card.svelte'

  const cards = [
    {
      title: 'Buying a new monitor',
      date: '2020-01-01',
      description: 'I want to buy a new monitor'
    },
    {
      title: 'Having a 30 min run',
      date: '2020-01-01',
      description: 'I had a 30 min run on the Paris Marathon'
    }
  ]
</script>

<main>
  <ul>
    {#each cards as card}
      <Card {card} />
    {/each}
  </ul>
</main>

<style>
  :root {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
      Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }

  main {
    text-align: center;
    padding: 1em;
    margin: 0 auto;
  }

  main ul {
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }

  @media (min-width: 480px) {
    h1 {
      max-width: none;
    }

    p {
      max-width: none;
    }
  }
</style>
