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
      <div class="coach">
        <div class="title">
          <span>教练</span>
          <span></span>
          <span >更多</span >
        </div>
        <div class="person">
          <div>allen</div>
          <div>allen</div>
          <div>allen</div>
          <div>allen</div>
        </div>
      </div>
      <div class="pic_wall">
        <div class="title">
          <span>照片墙</span>
          <span></span>
          <span >更多</span >
        </div>
        <div class="img_item">
          <div class="img"><img src="https://images.unsplash.com/photo-1551334787-21e6bd3ab135?w=640" alt=""></div>
          <div class="img"><img src="https://images.unsplash.com/photo-1551334787-21e6bd3ab135?w=640" alt=""></div>
          <div class="img"><img src="https://images.unsplash.com/photo-1551334787-21e6bd3ab135?w=640" alt=""></div>
          <div class="img"><img src="https://images.unsplash.com/photo-1551334787-21e6bd3ab135?w=640" alt=""></div>
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped>
.swiper {
  margin-left: 50rpx;
}

.title {
  display: flex;
  justify-content: space-between;
  padding: 10rpx 50rpx;
}

nav {
  display: flex;
  justify-content: space-around;
  height: 80rpx;
  line-height: 80rpx;
}

.person {
  display: flex;
  justify-content: space-around;
  height: 80rpx;
  line-height: 80rpx;
}

.img_item {
  display: flex;
  justify-content: flex-start;
  white-space: nowrap;
}

.img {
  height: 200rpx;
  width: 300rpx;
}

img image {
  height: 200rpx;
  width: 300rpx;
}
</style>

<script>
export default {
  data() {
    return {
      banner: [
        {
          image_url:
            "https://images.unsplash.com/photo-1551334787-21e6bd3ab135?w=640"
        },
        {
          image_url:
            "https://images.unsplash.com/photo-1551334787-21e6bd3ab135?w=640"
        },
        {
          image_url:
            "https://images.unsplash.com/photo-1551334787-21e6bd3ab135?w=640"
        },
        {
          image_url:
            "https://images.unsplash.com/photo-1551334787-21e6bd3ab135?w=640"
        }
      ]
    };
  },
  methods: {},
  mounted() {}
};
</script>
