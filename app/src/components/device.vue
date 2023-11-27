<template>
    <section class="center">
        
        <div class="m3-card" style="text-align: left;">
            <label>Model</label>
            <div>Example</div>
            <label>Android Version</label>
            <div>Example</div>
            <label>System Build Number</label>
            <div>Example</div>
            <label>Security Patch</label>
            <div>Example</div>
        </div>

        <div class="m3-card" v-if="false">
            <h2>No Device Found</h2>
        </div>

    </section>
</template>

<style scoped>
label {
    color: var(--foreground);
}
div {
    margin-bottom: 0.5em;
}
.m3-card {
    min-width: 45%;
}
</style>