<script>
  import FeedbackList from './lib/components/FeedbackList.svelte';

  const feedback = [
    {
      id:1,
      rating: 10,
      text: 'this feedback has recommendation of'
    },
    {
      id:2,
      rating: 9,
      text: 'this feedback has recommendation of'
    },
    {
      id:3,
      rating: 8,
      text: 'this feedback has recommendation of'
    }
  ];
</script>

<main>
  
  <h1>Vite + Svelte</h1>

  
  <FeedbackList {feedback}/>
  

 
</main>


