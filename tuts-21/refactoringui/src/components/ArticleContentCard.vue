<template>
    <div class="flex flex-col flex-1 overflow-hidden bg-white rounded-lg shadow-xl">    
        <a href="#!" class="block h-48 no-underline bg-cover" :style="{backgroundImage:`url(${image})`}">
        </a>
        <!-- :style="{backgroundImage:`url(${image})`}" 
        style="backgroundImage: url('https://www.refactoringui.com/img/homepage/article-tips.png')"-->
        <div class="flex flex-col justify-between flex-1 p-6">
            <h3 class="mb-4 text-lg font-bold">
                <a href="#!" class="no-underline hover:underline">                                
                    {{ title }}
                </a>
            </h3>
            <div>
                <a href="#!" class="inline-flex items-center no-underline">
                    <span class="mr-2 text-grey-dark">
                        twitter.com
                    </span>
                    <svg class="w-5 h-5 text-grey" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor">
                        <path d="M11 3a1 1 0 100 2h2.586l-6.293 6.293a1 1 0 101.414 1.414L15 6.414V9a1 1 0 102 0V4a1 1 0 00-1-1h-5z" />
                        <path d="M5 5a2 2 0 00-2 2v8a2 2 0 002 2h8a2 2 0 002-2v-3a1 1 0 10-2 0v3H5V7h3a1 1 0 000-2H5z" />
                    </svg>
                </a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "ArticleContentCard",
    props: {
        title: {
            String
        },
        image: {
            String
        }
    }
}
</script>

<style>

</style>