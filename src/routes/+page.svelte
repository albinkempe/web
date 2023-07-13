<main>
    <h1>Albin Kempe</h1>
    <p class="title">Computer Science Student at KTH Royal Institute of Technology</p>
</main>

<style lang="scss">
    @use 'variables';

    @import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;700&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Crimson+Text:ital,wght@0,400;0,600;0,700;1,400&display=swap');

    :global(body) {
        margin: 0;
        background-color: variables.$color-background;
    }

    main {
        height: 100vh;
        width: 100vw;

        font-family: 'Open Sans', sans-serif;
        font-size: 16px;
        
        color: variables.$color-text-1;

        margin: 0 auto;
        text-align: center;

        padding: 1em;
    }

    h1 {
        font-size: 300%;
        font-family: 'Crimson Text', serif;
        margin-top: 1em;
        margin-bottom: 0;
    }

    .title {
        margin-top: 0;
    }

</style>  