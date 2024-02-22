<title>My page title</title>
<link href="https://fonts.googleapis.com/css?family=Open+Sans+Condensed:300|Sonsie+One" rel="stylesheet" type="text/css">

<style>
  :root 
  {
    --primary-color: rgb(0, 0, 255);
    --secondary-color: rgb(0, 255, 255);
    --bg-color: rgb(255, 255, 255);
    --font-color: rgb(128, 128, 128);
    --heading-color: rgb(0, 0, 0);
  }

  [data-theme="dark"] 
  {
    --primary-color: rgb(0, 128, 0);
    --secondary-color: rgb(0, 255, 0);
    --bg-color: rgb(0, 0, 0);
    --font-color: rgb(128, 128, 128);
    --heading-color: rgb(255, 255, 255);
  }

header
  {
    background-color: var(--bg-color);
    color: var(--heading-color);
    text-align: center;
  }

  main 
  {
    text-align: center;
    background-color: var(--bg-color);
    color: var(--font-color);
  }

  button
  {
    background-color: var(--primary-color);
    color: var(--secondary-color);
  }

  main 
  {
  cursor: url("https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.hiclipart.com%2Ffree-transparent-background-png-clipart-ijcjx&psig=AOvVaw2vM4LtScBtCe7y8wiz5WN0&ust=1708668696920000&source=images&cd=vfe&opi=89978449&ved=0CBMQjRxqFwoTCLCTyoelvoQDFQAAAAAdAAAAABAO") 8 8, pointer;
  }

  .hover-container 
  {
  cursor: url("https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.hiclipart.com%2Ffree-transparent-background-png-clipart-ijcjx&psig=AOvVaw2vM4LtScBtCe7y8wiz5WN0&ust=1708668696920000&source=images&cd=vfe&opi=89978449&ved=0CBMQjRxqFwoTCLCTyoelvoQDFQAAAAAdAAAAABAO"), default;
  }

</style>

<header>
  <h1>Birds!</h1>
</header>



<main>

<img id="Image" src="http://www.outgrabe.net/bird00.jpg" alt="Pardalote">
    <p id="credit">Pardalote by fir0002 (CC-by-NC)</p>
    
 <button onclick="birdName('Pardalote')">Pardalote</button>
    <button onclick="birdName('Purple Swamp Hen')">Purple Swamp Hen</button>
    <button onclick="birdName('White-headed Stilt')">White-headed Stilt</button>
    <button onclick="birdName('Inland Thornbill')">Inland Thornbill</button>
    <button onclick="birdName('Rose Robin')">Rose Robin</button>  

</main>

<script>
    function birdName(name)
    {
        var birdImage = document.getElementById('Image');
        var credit = document.getElementById('credit');
    }

    switch (name)
    {
        case 'Pardalote':
            birdImage.src = 'http://www.outgrabe.net/bird00.jpg';
            credit.textContent = 'Pardalote by fir0002 (CC-by-NC)';
            break;
        case 'Purple Swamp Hen':
            birdImage.src = 'http://www.outgrabe.net/bird00.jpg';
            credit.textContent = 'Pardalote by fir0002 (CC-by-NC)';
            break;
        case 'White-headed Stilt':
            birdImage.src = 'http://www.outgrabe.net/bird02.jpg';
            credit.textContent = 'White-headed Stilt by JJ Harrison (CC-by-SA)';
            break;
        case 'Inland Thornbill':
            birdImage.src = 'http://www.outgrabe.net/bird03.jpg';
            credit.textContent = 'Inland Thornbill by Peter Jacobs (CC-by-SA)';
            break;
        case 'Rose Robin':
            birdImage.src = 'http://www.outgrabe.net/bird04.jpg';
            credit.textContent = 'Rose Robin by JJ Harrison (CC-by-SA)';
            break;
        default:
            break;
    }
</script>