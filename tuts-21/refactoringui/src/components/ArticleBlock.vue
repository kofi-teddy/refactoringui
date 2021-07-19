<template>
  <div class="container px-6 py-10 mx-auto">
      <div>
        <div class="flex items-baseline justify-between mb-10 border-b-2 border-grey-light">
            <span class="py-4 font-bold tracking-wide uppercase border-b-2 -mb-2px border-mindigo">Design Tips</span>
            <a href="#!" class="no-underline text-semibold text-mindigo-dark hover:underline">View All</a>
        </div>
        <div class="flex flex-wrap -mx-3">
            <div class="flex flex-col w-full px-3 mb-8 md:w-1/2 lg:w-1/3">
                <div class="flex flex-col flex-1 overflow-hidden bg-white rounded-lg shadow-lg">    
                    <a href="#!" class="block h-48 no-underline bg-cover" style="background-image:url('https://www.refactoringui.com/img/homepage/article-tips.png')">
                    </a>
                    <div class="flex flex-col justify-between flex-1 p-6">
                        <h3 class="mb-4 text-lg font-bold">
                            <a href="#!" class="no-underline hover:underline">                                
                                Think Outside the Database
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
            </div>
            <div class="flex flex-col w-full px-3 mb-8 md:w-1/2 lg:w-1/3">
                <div class="flex flex-col flex-1 overflow-hidden bg-white rounded-lg shadow-lg">    
                    <a href="#!" class="block h-48 no-underline bg-cover" style="background-image:url('https://www.refactoringui.com/img/homepage/article-tips.png')">
                    </a>
                    <div class="flex flex-col justify-between flex-1 p-6">
                        <h3 class="mb-4 text-lg font-bold">
                            <a href="#!" class="no-underline hover:underline">
                                User Fewer Borders
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
            </div>
            <div class="flex flex-col w-full px-3 mb-8 md:w-1/2 lg:w-1/3">
                <div class="flex flex-col flex-1 overflow-hidden bg-white rounded-lg shadow-lg">    
                    <a href="#!" class="block h-48 no-underline bg-cover" style="background-image:url('https://www.refactoringui.com/img/homepage/article-tips.png')">
                    </a>
                    <div class="flex flex-col justify-between flex-1 p-6">
                        <h3 class="mb-4 text-lg font-bold">
                           <a href="#!" class="no-underline hover:underline">Overlap Images to Add Depth</a>
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
            </div>
            <div class="flex flex-col w-full px-3 mb-8 md:w-1/2 lg:w-1/3">
                <article-content-card title="Hello world" image="https://www.refactoringui.com/img/homepage/article-tips.png"/>
            </div>
        </div>
      </div>
      <div>
        <div class="flex items-baseline justify-between mb-10 border-b-2 border-grey-light">
            <span class="py-4 font-bold tracking-wide uppercase border-b-2 -mb-2px border-mindigo">Design Tips</span>
            <a href="#!" class="no-underline text-semibold text-mindigo-dark hover:underline">View All</a>
        </div>
        <div class="flex flex-wrap -mx-3">
            <div class="flex flex-col w-full px-3 mb-8 md:w-1/2 lg:w-1/3" v-for="article in articles" :key="article.id">
                <article-content-card :title="article.title" :image="article.image"/>
            </div>
        </div>
      </div>
  </div>
</template>

<script>
import ArticleContentCard from './ArticleContentCard.vue'
import FooterBlock from './FooterBlock.vue'
export default {
    name: 'ArticleBlock',
    data() {
        return {
            articles: [
                {
                    id: 1,
                    title: "Cathsu",
                    image: 'https://www.refactoringui.com/img/homepage/article-tips.png'
                },
                {
                    id: 2,
                    title: "Cyto",
                    image: 'https://www.refactoringui.com/img/homepage/article-tips.png'
                },
                {
                    id: 3,
                    title: "Numbs",
                    image: 'https://www.refactoringui.com/img/homepage/article-tips.png'
                }
            ]
        }
    },
    components: { FooterBlock , ArticleContentCard},
}
</script>

<style>

</style>
