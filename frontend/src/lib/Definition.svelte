<script lang="ts">
    export let word;
    export let definition;
</script>

<div class="definition">
    <div>
        <span class="category">Word:</span>
        <span class="data">{word}</span>
    </div>
    <div>
        <span class="category">Definition:</span>
        <span class="data">{definition}</span>
    </div>
</div>

<style lang="scss">
    .definition {
        margin: 1em;
        padding: 1rem;
        border: white solid;
        border-radius: 1rem;
        background-color: rgb(36, 36, 36);
        width: 20%;
        text-align: left;
        .category {
            text-transform: uppercase;
            font-size: 1.2rem;
            font-weight: 100;
            line-height: 1.1;
            margin: 2rem auto;
        }
    }
</style>
