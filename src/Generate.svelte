<script lang="ts">
    import GenerateButton from "./lib/GenerateButton.svelte";
    import Definition from "./lib/Definition.svelte";
    let definitions: Array<{ word: string; definition: string }> = [];
    function generate() {
        definitions.push({ word: "test",definition: "Lorem ipsum"});
        definitions = definitions;
        console.log(definitions);
    }
</script>

<div>
    <GenerateButton callback={generate}/>
    <div class="definitions">
        {#each definitions as definition}
            <Definition word={definition.word} definition={definition.definition}/>
        {/each}
    </div>
</div>

<style lang="scss">
    .definitions {
        margin-top: 2em;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
</style>
