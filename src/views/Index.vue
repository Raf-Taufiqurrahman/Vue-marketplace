<template>
    <div class="w-full py-6 px-4">
        <div class="container mx-auto">
            <div class="flex flex-row overflow-x-auto gap-4 pb-8">
                <Slider />
            </div>
            <div class="flex flex-col">
                <h1 class="title">Category</h1>
                <p class="subTitle">This is a list of category</p>
            </div>
            <div class="grid grid-cols-2 lg:grid-cols-6 gap-4 py-5">
                <CategoryItem />
            </div>
            <div class="flex flex-col">
                <h1 class="title">Product</h1>
                <p class="subTitle">This is a list of product</p>
            </div>
            <div class="grid grid-cols-1 lg:grid-cols-3 gap-4 md:gap-14 py-5 pb-14 md:pb-0 items-start">
                <ProductItem />
            </div>
        </div>
    </div>
</template>

<script>
import Hero from '../components/Hero.vue';
import CategoryItem from '../components/CategoryItem.vue';
import ProductItem from '../components/ProductItem.vue'
import Slider from '../components/Slider.vue'
export default {
    components: { Hero, CategoryItem, ProductItem, Slider }
}
</script>