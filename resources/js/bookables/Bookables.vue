<template>
    <div>
        <item item-title="Cheap Villa" item-content="A very cheap villa" v-bind:price="1000"></item>
        <item item-title="Cheap Villa 2" item-content="A very cheap villa 2" :price="1500"></item>
    </div>
</template>

<script>
import BookableListitem from "./BookableListitem";

export default {
    components: {
        item: BookableListitem
    },
    beforeCreate() {
        console.log('before create');
    },
    created() {
        console.log('created');
    },
    beforeMount() {
        console.log('before mounted');
    },
    mounted() {
        console.log('mounted');
    },
    beforeDestroy() {
        console.log('before destroy');
    },
    destroyed() {
        console.log('destroyed');
    }
}
</script>
