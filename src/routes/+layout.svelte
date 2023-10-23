<slot />

<style>
    :root {
        --accent: #f00;
        --accent-light: #faa;
        --accent-dark: #500;

        --main: #222;
        --main-light: #333;
        --main-dark: #111;

        --main-text: #eee;

        --accent-gradient: linear-gradient(45deg, var(--accent), var(--accent-light) 30%, white 60%);
    }

    :global(body) {
        font-family: Helvetica, sans-serif;
        color: var(--main-text);
        background-color: var(--main);
        overflow: hidden;
    }
</style>