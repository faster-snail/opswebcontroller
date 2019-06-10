<template>
                <v-list>
                    <v-list-group
                            v-for="item in items"
                            :key="item.title"
                            v-model="item.active"
                            :prepend-icon="item.action"
                            no-action
                    >
                        <template v-slot:activator>
                            <v-list-tile>
                                <v-list-tile-content>
                                    <v-list-tile-title>{{ item.title }}</v-list-tile-title>
                                </v-list-tile-content>
                            </v-list-tile>
                        </template>
                        
                        <v-list-tile
                                v-for="subItem in item.items"
                                :key="subItem.title"
                                @click=""
                        >
                            <v-list-tile-content>
                                <v-list-tile-title>{{ subItem.title }}</v-list-tile-title>
                            </v-list-tile-content>
                            
                            <v-list-tile-action>
                                <v-icon>{{ subItem.action }}</v-icon>
                            </v-list-tile-action>
                        </v-list-tile>
                    </v-list-group>
                </v-list>
</template>

<script>
    export default {
        name: "List",
        data () {
            return {
                items: [
                    {
                        action: 'local_activity',
                        title: '大屏监控',
                        items: [
                            { title: 'List Item' }
                        ]
                    },
                    {
                        action: 'restaurant',
                        title: '服务器资源',
                        active: true,
                        items: [
                            { title: 'Breakfast & brunch' },
                            { title: 'New American' },
                            { title: 'Sushi' }
                        ]
                    },
                    {
                        action: 'school',
                        title: '软件部署',
                        items: [
                            { title: 'List Item' }
                        ]
                    },
                    {
                        action: 'directions_run',
                        title: '持续集成',
                        items: [
                            { title: 'List Item' }
                        ]
                    },
                    {
                        action: 'healing',
                        title: '日志输出',
                        items: [
                            { title: 'List Item' }
                        ]
                    },
                    {
                        action: 'content_cut',
                        title: '在线shell',
                        items: [
                            { title: 'List Item' }
                        ]
                    },
                    {
                        action: 'local_offer',
                        title: '操作记录',
                        items: [
                            { title: 'List Item' }
                        ]
                    }
                ]
            }
        }
    }
</script>

<style scoped>

</style>
