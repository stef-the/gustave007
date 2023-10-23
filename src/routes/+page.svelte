<script>
    const cards = [
        {
            title: 'Why we <3 Gussy',
            description: 'we don\'t',
            image: 'edouard0.jpg',
        },
        {
            title: 'Why Goonstave',
            description: ':)',
            image: 'gustave0.jpg',
        },
        {
            title: 'Why Goonstave',
            description: ':)',
            image: 'omarjmel0.jpg',
        },
        {
            title: 'Why Goonstave',
            description: ':)',
            image: 'gustave1.jpg',
        },
        {
            title: 'Why Goonstave',
            description: ':)',
            image: 'edouard1.jpg',
        },
    ]
</script>

<div id="header">
  <h1>Welcome to <b class="gradient">Gustave</b></h1>
  <i>wear the world gets it's fun</i>
</div>
{#each cards as card}
    <div class='card'>
        <div class='cardimage' style='background-image: url("https://raw.githubusercontent.com/stef-the/gustave007/main/static/{card.image}");'></div>
        <div>
            <h2>{card.title}</h2>
            <p>{card.description}</p>
        </div>
    </div>
{/each}

<style>
  .gradient {
    background-image: var(--accent-gradient);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-size: 400%;
  }
  #header {
    margin: 2.5rem;
    width: 100%;
    background-color: none;
    text-align: center;
  }
  #header i {
    font-size: 2rem;
  }
  h1, h2, p {
    margin: 0;
  }
  h1 {
    font-size: 5rem;
  }
  .card {
    background-color: var(--main-dark);
    margin: 2rem;
    padding: 1rem;
    height: 5rem;
    border-radius: 0.5rem;
    overflow: hidden;
    display: flex;
  }
  .card .cardimage {
    height: 5rem;
    width: 5rem;
    border-radius: 0.5rem;
    background-color: red;
    margin-right: 1rem;
    background-size: cover;
  }
  .card h2 {
    margin-bottom: 0.5rem;
  }
</style>
