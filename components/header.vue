<template>
    <section>
        <b-tabs position="is-centered" v-model="activeTab">
            <template v-for="(tab, index) in tabs">
                <b-tab-item
                    v-if="tab.displayed"
                    :key="index"
                    :label="tab.label">
                    {{ tab.content }}
                </b-tab-item>
            </template>
        </b-tabs>
    </section>
</template>

<script>
    export default {
        data() {
            return {
                activeTab: 0,
                showMusic: true,
                showBooks: false,
                multiline: true
            }
        },
        computed: {
            baseTabs() {
                return [
                    {
                        label: 'Pictures',
                        content: 'Pictures: Lorem ipsum dolor sit amet.',
                        displayed: true,
                    },
                    {
                        label: 'Music',
                        content: 'Music: Lorem ipsum dolor sit amet.',
                        displayed: true,
                    },
                    {
                        label: 'Videos',
                        content: 'Videos: Lorem ipsum dolor sit amet.',
                        displayed: true,
                    },
                    {
                        label: 'Games',
                        content: 'Games: Lorem ipsum dolor sit amet.',
                        displayed: true,
                    },
                    {
                        label: 'Comics',
                        content: 'Comics: Lorem ipsum dolor sit amet.',
                        displayed: true,
                    },
                    {
                        label: 'Movies',
                        content: 'Movies: Lorem ipsum dolor sit amet.',
                        displayed: true,
                    }
                ]
            },
            tabs() {
                const tabs = [...this.baseTabs]
                if (this.showBooks) {
                    tabs.splice(tabs.length - 1, 0, this.bookTab);
                }
                return tabs
            }
        }
    }
</script>

