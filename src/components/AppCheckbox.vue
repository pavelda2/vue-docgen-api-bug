<template>
    <div>
        <label>
            <input type="checkbox"/>
            <!-- @slot Label of checkbox -->
            <slot #label/>
        </label>
    </div>
</template>

<script>
    export default {
        name: "AppCheckbox"
    };
</script>