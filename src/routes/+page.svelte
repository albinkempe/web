<script lang="ts">
    import University from "../components/university.svelte";
</script>

<svelte:head>
    <title>@albinkempe</title>
</svelte:head>

<main>
    <h1>Albin Kempe</h1>

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

        <div class="projects">
            <div class="project">
                <h3>Best Project Award - Deep Learning in Data Science</h3>
                <p>Implemented a language model based on the transformer architeceture. Voted 'Best Project' out of 64 projects.</p>
                <p class="pdf"><a href="./assets/dl_project.pdf" target="_blank" rel="noopener noreferrer">A Re-Implementation and Exploration of the Transformer Architecture for Text Generation</a></p>
            </div>
            <div class="project">
                <h3>UFO - Information Visualization Project</h3>
                <p>Visualized UFO sightings in the U.S. for a group project.</p>
                <p class="pdf"><a href="https://useless-fisualization-operation.github.io/ufo-web/" target="_blank" rel="noopener noreferrer">Link to project website</a></p>
            </div>
            <div class="project">
                <h3>METAspexet 2023</h3>
                <p>Created graphical material such as merch, stickers and posters using Adobe Photoshop, Illustrator and InDesign for the annual METAspexet musical.</p>
            </div>
        </div>

        <University 
            university="KTH Royal Institue of Technology" 
            degree="BSc Computer Science"
            startDate="2019"
            endDate="2022"
            imageSrc="kth_logo.png"
            imageAlt="KTH logotype"
        />

        <div class="projects">
            <div class="project">
                <h3>Bachelor Thesis in Computer Vision</h3>
                <p>Investigated the effects of using pre-trained CNNs for skin cancer classification.</p>
                <p class="pdf"><a href="http://www.diva-portal.org/smash/record.jsf?dswid=-7473&faces-redirect=true&language=en&searchType=SIMPLE&query=albin+wikstr%C3%B6m+kempe&af=%5B%5D&aq=%5B%5B%5D%5D&aq2=%5B%5B%5D%5D&aqe=%5B%5D&pid=diva2%3A1703314&noOfRows=50&sortOrder=author_sort_asc&sortOrder2=title_sort_asc&onlyFullText=false&sf=all" target="_blank" rel="noopener noreferrer">Identifying Melanoma Using Transfer Learning and Convolutional Neural Networks: An investigation of skin disease pre-training</a></p>
            </div>
        </div>
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

        <div class="projects">
            <div class="project">
                <h3>Cloud Connector</h3>
                <p>I worked as a developer on a system integration project. I developed an efficent, stable and secure .NET software solution.</p>
            </div>
        </div>
    </section>

    <footer>
        Updated 2023-07-17
    </footer>

</main>

<style lang="scss">
    @use 'variables';
    @use 'fonts';

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

    a {
        color: variables.$color-text-1;
        margin: 0;
        font-size: 85%;
    }

    .projects {
        border-left: 2px solid;
        border-color: variables.$color-accent;
        margin: 0 0 3em 2em;
    }

    .project {
        margin-left: 2em;
        margin-bottom: 1.5em;
    }

    section {
        text-align: left;

    }

    h1 {
        font-size: 400%;
        line-height: 70%;
        font-family: 'Bright', sans-serif;
        margin: 0.2em 0 0.2em 0;
        font-weight: normal;
        font-style: normal;
    }

    h2 {
        margin-bottom: 0.3em;
    }

    h3 {
        font-size: 80%;
        margin-bottom: 0;
    }

    .pdf {
        margin: 0;
    }

    .project p {
        font-size: 80%;
        margin-top: 0.3em;
        margin-bottom: 0;
    }

    @media only screen and (min-width: 768px) {
        main {
            width: 50vw;
        }

        h1 {
            font-size: 800%;
            margin: 0.3em 0 0.3em 0;
        }
    }

    footer {
        font-size: 70%;
        color: darken(variables.$color-text-1, 30%);
        padding: 1em;
    }

</style>  