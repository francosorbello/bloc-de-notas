<script lang="ts">
/**
 * Input donde el usuario puede escribir texto
 * 
 * responsive: Define si el editor es responsive o no
 * width: ancho del medido en rem. Solo se utiliza si el editor no es responsive
 * height: medido en rem. Solo se utiliza si el editor no es responsive
 */
export default {
    name: "EditorText",
    props: {
        responsive: Boolean,
        width: Number,
        height: Number
    },
    methods: {
        onClick(){
            console.log(document.getElementById("h1piola")?.innerText)
        }
    }
}
</script>

<template>
    <div>
        <h1 contenteditable="true" id="h1piola">
            {{responsive}}
        </h1>
    <button @click="onClick">
        Click me
    </button>
    </div>
</template>