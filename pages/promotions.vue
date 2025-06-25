<script setup>
definePageMeta({
  layout: 'default'
})
useHead({
  title: '独家优惠与奖励 - 万搏娱乐 WGame',
  meta: [
    { name: 'description', content: '了解万搏娱乐最新优惠，包含首存加赠、免费旋转、每周再存奖励及体育过关加奖。' }
  ]
})
</script>

<template>
  <Container>
    <h1 class="mt-10 text-4xl font-bold text-zinc-800">独家优惠 & 奖励</h1>
    <table class="w-full mt-6 text-sm border-collapse">
      <thead>
        <tr class="border-b">
          <th class="p-2 text-left">奖励</th>
          <th class="p-2 text-left">规则</th>
          <th class="p-2 text-left">最高金额</th>
          <th class="p-2 text-left">投注要求</th>
        </tr>
      </thead>
      <tbody>
        <tr class="border-b">
          <td class="p-2">100 % 首存加赠</td>
          <td class="p-2">首次充值 ≥100 CNY</td>
          <td class="p-2">1,000 CNY</td>
          <td class="p-2">25 × 奖金</td>
        </tr>
        <tr class="border-b">
          <td class="p-2">新人 150 次免费旋转</td>
          <td class="p-2">完成首存后 24h 内领取</td>
          <td class="p-2">—</td>
          <td class="p-2">20 × 中奖额</td>
        </tr>
        <tr class="border-b">
          <td class="p-2">每周再存 50 %</td>
          <td class="p-2">周五-周日，最低 200 CNY</td>
          <td class="p-2">888 CNY</td>
          <td class="p-2">15 × 奖金</td>
        </tr>
        <tr>
          <td class="p-2">体育 70 % 复式过关加奖</td>
          <td class="p-2">≥2 场组合投注</td>
          <td class="p-2">28,000 CNY</td>
          <td class="p-2">按注单</td>
        </tr>
      </tbody>
    </table>
    <p class="mt-4 text-xs text-zinc-500">*所有优惠须在注册后 30 天内申领，适用《奖金条款》及地区限制。详情见“用户协议”。*</p>
  </Container>
</template>
