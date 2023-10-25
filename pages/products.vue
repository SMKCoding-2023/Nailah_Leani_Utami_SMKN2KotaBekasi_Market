<script lang="ts" setup>
import navbar from '../components/Header.vue';
import copyright from '../components/Footer.vue';
import { products } from '~/composables/constants/products';
const selectedCategory = ref("");
const allProducts = computed(() => {
    if (selectedCategory.value) {
        return products.filter((item) => item.category === selectedCategory.value);
    }
    return products;
});
</script>
<template>
    <navbar />
    <section>
        <div class="container">
            <div class="py-10 ml-20">
                <div class="mb-6 flex justify-end gap-6">
                    <Dropdown @selected-category="selectedCategory = $event" />
                </div>
                <div class="flex gap-6 flex-wrap mx-auto">
                    <template v-for="(item, index) in allProducts" :key="index">
                        <CardsCardProduct :product="item" class="w-[calc(100%/4-18px)]" />
                    </template>
                </div>
            </div>
        </div>
    </section>
    <br><br><br><br><br><br>
    <copyright />
</template>