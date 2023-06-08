<script setup>
    const props = defineProps(['getOperacao']);
</script>

<template>
    <div class="p-2 bg-success bg-opacity-25 rounded-3 text-center m-auto" style="width: 296px;">
        <div class="col-md-12">
            <output name="result" style="font-size: large; font-weight: 700;">{{ 'Resultado: ' + props.getOperacao }}</output>
        </div>
    </div>
</template>
