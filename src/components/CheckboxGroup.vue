<template>
    <div>
        <app-checkbox v-for="option in options" :key="option">
            <template #label>
                <!-- @slot Content of checkbox label delegated to the AppCheckbox component -->
                <slot #label>{{option}}</slot>
            </template>
        </app-checkbox>
    </div>
</template>

<script>
    import AppCheckbox from "./AppCheckbox";
    export default {
        name: "CheckboxGroup",
        components: {AppCheckbox},
        props: {
            options: {
                type: Array,
                required: true
            },
        },
    };
</script>