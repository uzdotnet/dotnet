<template>
  <Layout>
    <div class="pt-8 md:pt-16">
      <div class="flex flex-col items-center">
        <div class="flex flex-col items-center mb-2 text-ui-primary">
          <!-- <Logo width="120"  /> -->
          <!-- <h2 class="text-3xl text-6xl font-black tracking-tighter border-none">
            DOT-NET.UZ
          </h2> -->
        </div>
        <h1 class="text-4xl text-center lg:text-5xl">
          .NET Uzbekistan Community
        </h1>
        <p class="text-xl font-medium text-center">
          Microsoft .NET platformasi bo'yicha O'zbekistonda ilk dokumentatsiya
        </p>

        <div class="py-4">
          <code class="block px-4 py-1 select-all bg-ui-border text-ui-typo">Console.WriteLine("Salom Dunyo!");</code>
        </div>

        <div class="flex justify-center mt-8">
          <a
            href="https://docs.dot-net.uz/"
            class="flex items-center px-6 py-4 ml-auto text-2xl font-bold leading-none text-white border rounded-lg shadow-lg bg-ui-primary border-ui-primary transition-all duration-200 ease-out transform hover:shadow-xl hover:-translate-y-1"
          >
            Boshlash
            <ArrowRightCircleIcon class="ml-4" size="1x" />
          </a>
        </div>

        <p class="mt-8 text-center">
          Ochiq manba tizimi asosida GPL-3.0 litsenziyalangan
        </p>

      </div>

      <div class="pt-8 mx-auto mt-8 border-t md:mt-16 md:pt-16 border-top border-ui-border max-w-screen-sm"></div>

      <div class="flex flex-wrap justify-center -mx-4">
        <div class="flex flex-col items-center w-full px-4 mb-8 text-center md:w-1/3">
          <ZapIcon size="3x" class="mb-6 text-ui-primary" />
          <h3 class="font-bold tracking-wide uppercase text-ui-primary">
            Juda tez
          </h3>
          <p class="text-lg text-left">
            Web sahifa o'z ichiga eng zamonaviy va oxirgi javascript frameworklarni olib, web sayt tasavvur qilib bo'lmas darajada tez ishlashini ta'minlaydi. <span class="border-b border-dashed border-ui-primary text-ui-primary">Be hazil</span>.
          </p>
        </div>

        <div class="flex flex-col items-center w-full px-4 mb-8 text-center md:w-1/3">
          <SearchIcon size="3x" class="mb-6 text-ui-primary" />
          <h3 class="font-bold tracking-wide uppercase text-ui-primary">
            Qidiruv bo'limi
          </h3>
          <p class="text-lg text-left">
            Web sahifa zamonaviy va aqlli qidirish sxemalarini ishlatadi. Istalgan ma'lumotni <span class="border-b border-dashed border-ui-primary text-ui-primary">bir zumda</span> qidirib toping.
          </p>
        </div>

        <div class="flex flex-col items-center w-full px-4 mb-8 text-center md:w-1/3">
          <MoonIcon size="3x" class="mb-6 text-ui-primary" />
          <h3 class="font-bold tracking-wide uppercase text-ui-primary">
            Tungi qiyofa
          </h3>
          <p class="text-lg text-left">
            Kechqurun ko'zingiz og'ritib qo'ydimi? Tungi qiyofani yoqing va web sahifadan istalgancha bezarar foydalaning.
          </p>
        </div>
      </div>

    </div>
  </Layout>
</template>

<script>
import Logo from '@/components/Logo';
import { ArrowRightCircleIcon, ZapIcon, CodeIcon, MoonIcon, SearchIcon } from 'vue-feather-icons';

export default {
  components: {
    Logo,
    ArrowRightCircleIcon,
    ZapIcon,
    CodeIcon,
    MoonIcon,
    SearchIcon
  },

  metaInfo() {
    const title = '.NET Uzbekistan';
    const description = 'Microsoft .NET platformasi bo\'yicha O\'zbekistonda ilk dokumentatsiya';

    return {
      title: title,
      meta: [
        {
          name: 'description',
          content: description
        },
        {
          key: 'og:title',
          name: 'og:title',
          content: title,
        },
        {
          key: 'twitter:title',
          name: 'twitter:title',
          content: title,
        },
        {
          key: 'og:description',
          name: 'og:description',
          content: description,
        },
        {
          key: 'twitter:description',
          name: 'twitter:description',
          content: description,
        },
      ]
    }
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
