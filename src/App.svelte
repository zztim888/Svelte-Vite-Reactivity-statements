<script>
  let count =0;

  $: if(count>=10){
    alert("the count is bigger than 10");
    count =9;
  }

  function handleClick(){
    count += 1;
  }
</script>

<h1>reactivity/ statements</h1>

<button on:click={handleClick}>
count {count} {count === 1 ? 'time':'times'}
</button>

<p>click more than 9x to see what happens</p>
