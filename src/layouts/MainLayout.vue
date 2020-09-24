<template>
    <div>
        <Sidebar/>
        <Dropdown/>
        <router-view/>
    </div>
</template>

<script>
import Sidebar from '@/components/Sidebar.vue'
import Dropdown from '@/components/Dropdown.vue'
export default {
    components: {
        Sidebar,
        Dropdown
    }
}
</script>
