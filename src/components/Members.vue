<template>
    <ul id="member-list">
        <li v-for="member in members">
            <img
                :src="require(`@/assets/images/members/${member.cover_url}.jpg`)"
                :alt="member.name"
            />
            <p>{{ member.name }}</p>
        </li>
    </ul>
</template>

<script lang="ts">
import Vue from 'vue';
import { Component } from 'vue-property-decorator';
import { Member } from '../models/Member';

@Component
export default class Members extends Vue {
  private members: Array<Member> = [];

  mounted() {
    this.members.push({
      name: 'Chika Takami',
      slug: 'chika_takami',
      cover_url: 'chika_takami',
    });

    this.members.push({
      name: 'Dia Kurosawa',
      cover_url: 'dia_kurosawa',
      slug: 'dia_kurosawa',
    });

    this.members.push({
      name: 'Hanamaru Kunikida',
      cover_url: 'hanamaru_kunikida',
      slug: 'hanamaru_kunikida',
    });

    this.members.push({
      name: 'Kanan Matsuura',
      cover_url: 'kanan_matsuura',
      slug: 'kanan_matsuura',
    });

    this.members.push({
      name: 'Mari Ohara',
      cover_url: 'mari_ohara',
      slug: 'mari_ohara',
    });

    this.members.push({
      name: 'Riko Sakurauchi',
      cover_url: 'riko_sakurauchi',
      slug: 'riko_sakurauchi',
    });

    this.members.push({
      name: 'Ruby Kurosawa',
      cover_url: 'ruby_kurosawa',
      slug: 'ruby_kurosawa',
    });

    this.members.push({
      name: 'Yoshiko Tsushima',
      cover_url: 'yoshiko_tsushima',
      slug: 'yoshiko_tsushima',
    });

    this.members.push({
      name: 'You Watanabe',
      cover_url: 'you_watanabe',
      slug: 'you_watanabe',
    });

    console.log(this.members);
  }
}
</script>

<style scoped lang="scss">
ul {
  list-style: none;
}

  li {
    display: inline-flex;

  }

  p {
    display: inline-flex;
  }
</style>
