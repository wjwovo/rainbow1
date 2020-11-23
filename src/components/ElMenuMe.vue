<template>
    <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
        <el-menu-item index="/">主页</el-menu-item>
        <el-menu-item index="/teacher">筑梦师</el-menu-item>
        <el-menu-item index="/course">课程</el-menu-item>
    </el-menu>
</template>

<script>
    export default {
        name: "ElMenuMe",
        props: {
            default_active: String
        },
        data() {
            return {
                activeIndex: this.props.default_active,
            };
        },
        methods: {
            handleSelect(key, keyPath) {
                this.$router.push(key)
            }
        }
    }
</script>

<style scoped>

</style>