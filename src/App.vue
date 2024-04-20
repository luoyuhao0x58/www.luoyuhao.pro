<script setup lang="ts">
import Profile from './components/Profile.vue';
import LinkButton from './components/LinkButton.vue';
</script>

<template>
  <!--  -->
  <div class="container mx-auto w-full flex flex-col min-h-screen justify-center items-center">
    <div class="min-w-fit max-w-screen-sm">
      <div class=" flex flex-col justify-center items-center">
        <picture>
          <source srcset="./assets/avatar.avif" type="image/avif" />
          <source srcset="./assets/avatar.webp" type="image/webp" />
          <img src="./assets/avatar.png" class="logo" alt="avatar" />
        </picture>
        <Profile msg="Luo Yuhao" />
        <div class="text-lg lg:w-4/6 sm:w-9/10 sm:border-dashed border-1 p-1em rounded-2xl">
          <p>你好，欢迎来到我的小站！</p>
          <p>我是一名工作多年的大龄程序员，平常的工作主要是后端开发为主，主要开发语言是 Python。</p>
          <p>在某一天，我突然想到作为一个互联网老兵居然连个自己的站点都没有，很是说不过去，于是便有了这个站，顺便也把开发这个站点作为重新学习前端的练手项目。</p>
          <p>想法是把 www 作为站点入口，联结博客和自己的工具集，或者其他自己想展示和分享东西。</p>
          <p>希望随着时间的推移，能输出比较多的原创内容，主要是把日常自己所想总结出来备忘。如果这些内容刚好能带给路过的你一点启发，也算有了点价值了。</p>
        </div>
        <div class="m-1.5em lg:w-2.5/6 grid grid-flow-col justify-around ">
          <LinkButton msg="联系我" url="&#x6d;&#x61;&#x69;&#x6c;&#x74;&#x6f;&colon;&#x69;&commat;&#x6d;&#x61;&#x69;&#x6c;&period;&#x6c;&#x75;&#x6f;&#x79;&#x75;&#x68;&#x61;&#x6f;&period;&#x70;&#x72;&#x6f;"/>
          <LinkButton msg="博客" url="https://blog.luoyuhao.pro"/>
          <LinkButton msg="工具集" url="https://tools.luoyuhao.pro"/>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.logo {
  height: 12em;
  will-change: filter;
  transition: filter 300ms;
  filter: drop-shadow(0 0 2px #FFF);
}
.logo:hover {
  /* filter: drop-shadow(0 0 2em #ECCED0); */
  filter: drop-shadow(0 0 2em #FFF);
}
</style>
