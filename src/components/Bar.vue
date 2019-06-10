<template>
        <v-toolbar
                color="black"
                dark
        >
            <v-toolbar-title>OpsBible 自动化运维平台</v-toolbar-title>
        
            <v-divider
                    class="mx-3"
                    inset
                    vertical
            ></v-divider>
        
            <span class="subheading">首页</span>
        
            <v-spacer></v-spacer>
        
            <v-toolbar-items>
                <v-btn flat>
                    专业导航
                </v-btn>
            
                <v-divider vertical></v-divider>
            
                <v-btn flat>
                    技术博客
                </v-btn>
            
                <v-divider vertical></v-divider>
            
                <v-btn flat>
                    监控
                </v-btn>
            
                <v-divider vertical></v-divider>
            </v-toolbar-items>
        
            <v-toolbar-side-icon></v-toolbar-side-icon>
        </v-toolbar>
</template>

<script>
    export default {
        name: 'Bar'
    }
</script>

<style scoped>
</style>
