<script>
  import svelteLogo from './assets/svelte.svg'
  import Counter from './lib/Counter.svelte'

  const feedback = [
    {
      id:1,
      rating: 10,
      text: 'this feedback has recommendation of 10'
    },
    {
      id:2,
      rating: 9,
      text: 'this feedback has recommendation of 9'
    },
    {
      id:3,
      rating: 8,
      text: 'this feedback has recommendation of 8'
    }
  ];
</script>

<main>
  
  <h1>Vite + Svelte</h1>

  <div class="card">
    <Counter />
  </div>

 
</main>


