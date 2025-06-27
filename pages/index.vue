<script setup>
import Hero from '@/components/Hero.vue'
import Testimonials from '@/components/Testimonials.vue'

definePageMeta({
  layout: 'default'
})
useHead({
  title: '万搏娱乐 WGame — 全球玩家信赖的一站式在线娱乐平台',
  meta: [
    { name: 'description', content: '万搏娱乐提供体育竞猜、真人娱乐、电子游戏、彩票投注等多元化博彩服务，支持极速秒提与 24×7 中文客服。立即注册尊享首存加赠与免费旋转。' }
  ]
})

const hero = {
  title: '万搏娱乐 WGame — 全球玩家信赖的一站式在线娱乐平台',
  description: '立即注册，尊享 100 % 首存加赠 + 150 次免费旋转，极速秒提、24 × 7 中文客服！',
  image: '/images/hero.jpg',
  imageAlt: 'WGame hero banner',
  buttons: [
    { label: '注册拿奖金', url: '/register' },
    { label: '试玩体验', url: '/demo' }
  ]
}

const testimonials = [
  {
    quote: 'WGame 的返水最高，提取也快，我每天都来玩！',
    author: { name: '张伟', title: '资深玩家', avatar: '/images/person-1.jpg' }
  },
  {
    quote: '客服响应迅速，游戏体验一流。',
    author: { name: '李娜', title: '忠实用户', avatar: '/images/person-2.jpg' }
  },
  {
    quote: '在这里投注体育赛事感觉非常安全可靠。',
    author: { name: 'Chris', title: 'Sports Bettor', avatar: '/images/person-3.jpg' }
  }
]

const socials = [
  { label: 'X', url: 'https://x.com/fmmfm_kunrt' },
  { label: 'LinkedIn', url: 'https://www.linkedin.com/in/wgame' },
  { label: 'YouTube', url: 'https://www.youtube.com/@WGame_bet' },
  { label: 'Google', url: 'https://share.google/mMWvUtDGr3eztUirZ' },
  { label: 'TikTok', url: 'https://www.tiktok.com/@user002490470' },
  { label: 'Facebook', url: 'https://www.facebook.com/WGamebet1' }
]
</script>

<template>
  <Container>
    <Hero
      :title="hero.title"
      :description="hero.description"
      :image="hero.image"
      :imageAlt="hero.imageAlt"
      :buttons="hero.buttons"
    />

    <section class="mb-8">
      <h2 class="text-3xl font-bold text-zinc-800">为什么选择 WGame？</h2>
      <ul class="mt-4 space-y-2 list-disc ml-6 text-zinc-600">
        <li><strong>高额返水</strong>：每日最高 1.5 %，即时派发，自动到账</li>
        <li><strong>秒存秒提</strong>：支持 Alipay / WeChat / USDT / Visa，平均到账 60 秒</li>
        <li><strong>顶尖游戏</strong>：真人视讯、体育投注、老虎机、棋牌… 超 5,000+ 认证 RNG 游戏</li>
        <li><strong>安全合规</strong>：256-bit SSL + 独立 RNG 审计 + 多重 KYC/AML 机制</li>
        <li><strong>VIP 俱乐部</strong>：七级晋升，专属经理、生日现金券、奢华实物奖品</li>
      </ul>
    </section>

    <blockquote class="text-sm text-zinc-500 mb-8">
      <strong>Responsible Gaming</strong>：未满 18 岁及高风险人群请勿参与。本平台支持 GamCare、BeGambleAware 等公益组织。
    </blockquote>

    <div class="flex flex-wrap gap-4 mb-10">
      <NuxtLink to="/register" class="px-6 py-3 text-white bg-green-600 rounded-sm hover:bg-gray-800">注册拿奖金</NuxtLink>
      <NuxtLink to="/demo" class="px-6 py-3 text-white bg-gray-600 rounded-sm hover:bg-gray-800">试玩体验</NuxtLink>
    </div>

    <div class="flex flex-wrap gap-4 mb-20">
      <a v-for="s in socials" :key="s.url" :href="s.url" target="_blank" rel="noopener" class="text-sm underline text-blue-600 hover:text-blue-800">
        {{ s.label }}
      </a>
    </div>

    <Testimonials :title="'玩家好评'" :items="testimonials" />
  </Container>
</template>
