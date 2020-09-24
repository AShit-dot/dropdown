<template>
    <div class="dropdown">
        <button class="btn btn-secondary dropdown-toggle" ref="dropdown" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
            Dropdown button
        </button>
        <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
            <a class="dropdown-item" href="#">Action</a>
            <a class="dropdown-item" href="#">Another action</a>
            <a class="dropdown-item" href="#">Something else here</a>
        </div>
    </div>
</template>

<script>
import $ from 'jquery'
export default {
    mounted () {
        $(this.$refs.dropdown).dropdown()
    }
}
</script>

<style lang="scss">
.dropdown {
    position: absolute;
    // margin: 10px 10px 0 0;
}
</style>