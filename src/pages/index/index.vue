<template>
  <div>
    <header>
      <div class="swiper">
        <swiper class="swiper-container" indicator-dots="true" autoplay="true" interval="3000" circular="true" duration="500">
          <block v-for="(item, index) in banner " :key="index">
            <swiper-item class="swiper-item">
              <image :src="item.image_url" class="slide-image" />
            </swiper-item>
          </block>
        </swiper>
      </div>
    </header>
    <section>
      <nav>
        <div>打卡</div>
        <div>场馆信息</div>
        <div>特色课程</div>
      </nav>
      <div>

      </div>
    </section>
  </div>
</template>

<style scoped>
  .swiper {
    margin-left: 50rpx;
  }

  nav {
    display: flex;
    justify-content: space-around;
    height: 80rpx;
    line-height: 80rpx;
  }
</style>

<script>
export default {
  data() {
    return {
      banner: [
        {image_url: 'https://images.unsplash.com/photo-1551334787-21e6bd3ab135?w=640'},
        {image_url: 'https://images.unsplash.com/photo-1551334787-21e6bd3ab135?w=640'},
        {image_url: 'https://images.unsplash.com/photo-1551334787-21e6bd3ab135?w=640'},
        {image_url: 'https://images.unsplash.com/photo-1551334787-21e6bd3ab135?w=640'},
      ],
    };
  },
  methods: {},
  mounted() {}
};
</script>
