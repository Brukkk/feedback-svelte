<script>
  import FeedbackList from './lib/components/FeedbackList.svelte';

  let feedback = [
    {
      id:1,
      rating: 10,
      text: '"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse."'
    },
    {
      id:2,
      rating: 9,
      text: '"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse."'
    },
    {
      id:3,
      rating: 8,
      text: '"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse."'
    }
  ];

  const deleteFeedback = (e) => {
    const itemId = e.deatil;
    feedback = feedback.filter(fb => fb.id != itemId)
  }
</script>

<main>
  
  <h1>Vite + Svelte</h1>

  
  <FeedbackList {feedback} on:feedback-delete={deleteFeedback}/>
  

 
</main>


