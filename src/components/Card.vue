<template>
    <div class="card">
        <div id="header">
            <slot name="header"></slot>
        </div>
        <div class="rest">
            <div id="title">
                <slot name="title"></slot>
            </div>
            <div id="body">
                <slot name="body"></slot>
            </div>
            <div id="footer">
                <slot name="footer"></slot>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "CardTemplate",
}
</script>

<style>  
</style>