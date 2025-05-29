<template>
  <div>
    <!-- Breadcrumb -->
    <Breadcrumb breadcrumb="Bus Map" />

    <div class="mt-4">
      <div class="p-6 bg-white rounded-md shadow-md">
        <h2 class="text-lg font-semibold text-gray-700 capitalize mb-4">
          Bus Map
        </h2>

        <div class="w-full h-[600px] bg-gray-100 rounded-lg">
          <!-- 여기에 지도 컴포넌트가 들어갈 예정입니다 -->
          <div class="w-full h-full flex items-center justify-center">
            <p class="text-gray-500">지도가 로드되는 중입니다...</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { onMounted } from 'vue';
import Breadcrumb from '../partials/AppBreadcrumb.vue';

onMounted(() => {
  // 새 탭에서 열기
  window.open(window.location.href, '_blank');
});
</script> 