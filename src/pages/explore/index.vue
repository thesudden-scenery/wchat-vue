<template>
  <div class="explore">
    <group>
      <cell :is-link="true">
        <span slot="title">{{ titles[0] }}</span>
        <img slot="icon" :src="icons[0]" alt="">
      </cell>
    </group>
    <group>
      <cell :is-link="true">
        <span slot="title">{{ titles[1] }}</span>
        <img slot="icon" :src="icons[1]" alt="">
      </cell>
      <cell :is-link="true">
        <span slot="title">{{ titles[2] }}</span>
        <img slot="icon" :src="icons[2]" alt="">
      </cell>
    </group>
    <group>
      <cell :is-link="true">
        <span slot="title">{{ titles[3] }}</span>
        <img slot="icon" :src="icons[3]" alt="">
      </cell>
      <cell :is-link="true">
        <span slot="title">{{ titles[4] }}</span>
        <img slot="icon" :src="icons[4]" alt="">
      </cell>
    </group>
    <group>
      <cell :is-link="true">
        <span slot="title">{{ titles[5] }}</span>
        <img slot="icon" :src="icons[5]" alt="">
      </cell>
      <cell :is-link="true">
        <span slot="title">{{ titles[6] }}</span>
        <img slot="icon" :src="icons[6]" alt="">
      </cell>
    </group>
    <group>
      <cell :is-link="true">
        <span slot="title">{{ titles[7] }}</span>
        <img slot="icon" :src="icons[7]" alt="">
      </cell>
    </group>
  </div>
</template>

<script>
import { Group, Cell } from 'vux'

import friend from './icons/w-explore-friend.svg'
import sao from './icons/w-explore-sao.svg'
import shake from './icons/w-explore-shake.svg'
import nearby from './icons/w-explore-nearby.svg'
import bottle from './icons/w-explore-bottle.svg'
import shop from './icons/w-explore-shop.svg'
import game from './icons/w-explore-game.svg'
import app from './icons/w-explore-app.svg'

export default {
  name: 'explore',
  data () {
    return {
      icons: [friend, sao, shake, bottle, nearby, shop, game, app],
      titles: ['朋友圈', '扫一扫', '摇一摇', '漂流瓶', '附近的人', '购物', '游戏', '小程序']
    }
  },
  components: {
    Cell,
    Group
  }
}
</script>
