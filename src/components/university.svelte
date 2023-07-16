<script lang="ts">
    // @ts-nocheck
    export let university;
    export let degree;
    export let startDate;
    export let endDate;
    export let imageSrc;
    export let imageAlt;

</script>

<div class="card">
    <div class="flex-horizontal">
        <img src="{imageSrc}" alt="{imageAlt}">
        <div class="flex-vertical">
            <p class="degree">{degree}</p>
            <p class="uni">{university}</p>
            <p class="date">{startDate} - {endDate}</p>
        </div>
    </div>
</div>

<style lang="scss">
    @use '../routes/variables';

    .card {
        background-color: variables.$color-card;
        padding: 0.8em;
        border-radius: 0.3em;
        margin: 1em 0;
        box-shadow: 1px 1px 5px rgb(21, 21, 21);

        img {
            height: 4em;
            width: 4em;
            border-radius: 0.1em;
        }
    }

    .uni, .degree, .date {
        margin: 0;
        text-align: left;
        line-height: 90%;
    }

    .degree {
        font-weight: bold;
    }

    .uni {
        font-size: 90%;
    }

    .date {
        font-size: 70%;
        color: darken(variables.$color-text-1, 30%);
    }

    .flex-horizontal {
        display: flex;
        flex-direction: row;
    }

    .flex-vertical {
        display: flex;
        flex-direction: column;
        margin-left: 2em;
        height: 4em;
        justify-content: space-between;
    }
</style>