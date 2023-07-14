<script>
    import University from "../components/university.svelte";
</script>

<main>
    <h1>Albin Kempe</h1>

    <section class="bio">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </section>

    <section>
        <h2>Education</h2>
        <University 
            university="KTH Royal Institue of Technology" 
            degree="MSc Computer Science, Interaction Design"
            startDate="2022"
            endDate="2024"
            imageSrc="kth_logo.png"
            imageAlt="KTH logotype"
        />
        <University 
            university="KTH Royal Institue of Technology" 
            degree="BSc Computer Science"
            startDate="2019"
            endDate="2022"
            imageSrc="kth_logo.png"
            imageAlt="KTH logotype"
        />
    </section>

    <section>
        <h2>Work Experience</h2>
        <University 
            university="Thermo Fisher Scientific" 
            degree="Digital Service Intern"
            startDate="2022"
            endDate="2023"
            imageSrc="tfs_logo.jpeg"
            imageAlt="TFS logotype"
        />
    </section>

    <footer>
        2023
    </footer>

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
        min-height: 100vh;
        width: 100vw;

        display: flex;
        flex-direction: column;

        font-family: 'Open Sans', sans-serif;
        font-size: 16px;
        
        color: variables.$color-text-1;

        margin: 0 auto;
        text-align: center;

        padding: 1em;
    }

    section {
        text-align: left;

    }

    .bio {
        margin: 0 1em;
    }

    h1 {
        font-size: 300%;
        font-family: 'Crimson Text', serif;
        margin-top: 1em;
        margin-bottom: 1em;
    }

    h2 {
        margin-bottom: 0.3em;
    }

    @media only screen and (min-width: 768px) {
        main {
            width: 50vw;
        }
    }

    footer {
        font-size: 70%;
        color: darken(variables.$color-text-1, 30%);
        padding: 1em;
    }

</style>  