<template>
    <a-layout id="components-layout-demo-top-side">
        <a-layout-header class="header">
            <div class="logo"/>
            <a-menu
                theme="dark"
                mode="horizontal"
                :default-selected-keys="['2']"
                :style="{ lineHeight: '64px' }"
            >
                <a-menu-item key="1">
                    Vue
                </a-menu-item>
                <a-menu-item key="2">
                    React
                </a-menu-item>
            </a-menu>
        </a-layout-header>
        <a-layout-content style="padding: 0 50px">
            <a-breadcrumb v-if="false" style="margin: 16px 0">
                <a-breadcrumb-item>Home</a-breadcrumb-item>
                <a-breadcrumb-item>List</a-breadcrumb-item>
                <a-breadcrumb-item>App</a-breadcrumb-item>
            </a-breadcrumb>
            <a-layout v-if="false" style="padding: 24px 0; background: #fff">
                <a-layout-sider width="200" style="background: #fff">
                    <a-menu
                        mode="inline"
                        :default-selected-keys="['1']"
                        :default-open-keys="['sub1']"
                        style="height: 100%"
                    >
                        <a-sub-menu key="sub1">
                            <span slot="title"><a-icon type="user"/>subnav 1</span>
                            <a-menu-item key="1">
                                option1
                            </a-menu-item>
                            <a-menu-item key="2">
                                option2
                            </a-menu-item>
                            <a-menu-item key="3">
                                option3
                            </a-menu-item>
                            <a-menu-item key="4">
                                option4
                            </a-menu-item>
                        </a-sub-menu>
                        <a-sub-menu key="sub2">
                            <span slot="title"><a-icon type="laptop"/>subnav 2</span>
                            <a-menu-item key="5">
                                option5
                            </a-menu-item>
                            <a-menu-item key="6">
                                option6
                            </a-menu-item>
                            <a-menu-item key="7">
                                option7
                            </a-menu-item>
                            <a-menu-item key="8">
                                option8
                            </a-menu-item>
                        </a-sub-menu>
                        <a-sub-menu key="sub3">
                            <span slot="title"><a-icon type="notification"/>subnav 3</span>
                            <a-menu-item key="9">
                                option9
                            </a-menu-item>
                            <a-menu-item key="10">
                                option10
                            </a-menu-item>
                            <a-menu-item key="11">
                                option11
                            </a-menu-item>
                            <a-menu-item key="12">
                                option12
                            </a-menu-item>
                        </a-sub-menu>
                    </a-menu>
                </a-layout-sider>
                <a-layout-content :style="{ padding: '0 24px', minHeight: '280px' }">
                    Content
                </a-layout-content>
            </a-layout>
        </a-layout-content>
        <a-layout-footer style="text-align: center">
            Ant Design ©2018 Created by Ant UED
        </a-layout-footer>
    </a-layout>
</template>

<style lang="scss" scoped>
@import "style";
</style>
