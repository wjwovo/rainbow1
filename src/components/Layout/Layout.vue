<template>
    <div id="layout">
        <el-container>
            <el-header>
                <Navigation/>
            </el-header>
            <el-main>
                <router-view/>
            </el-main>
            <el-footer>
                <Footer/>
            </el-footer>
        </el-container>
    </div>
</template>

<script>

    import Navigation from "./Navigation";
    import Footer from "./Footer";
    export default {
        name: "Layout",
        components: {Footer, Navigation}
    }
</script>

<style scoped>

</style>