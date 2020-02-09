<template>
  <v-content>
    <v-container>

    <!-- パンくずリスト -->
    <div>
    <v-breadcrumbs :items="items" divider=">"></v-breadcrumbs>
    </div>
    <!-- パンくずリスト終わり -->

    <!-- スライド -->
    <v-carousel>
    <v-carousel-item
      v-for="(color, i) in colors"
      :key="color"
    >
    <v-sheet
      :color="color"
      height="100%"
      tile
    >
    <v-row
      class="fill-height"
      align="center"
      justify="center"
    >
    <div class="display-3">すらいど {{ i + 1 }}</div>
    </v-row>
    </v-sheet>
    </v-carousel-item>
    </v-carousel>
    <!-- スライド終わり -->

    <!-- タイル -->
    <v-layout wrap>
      <v-flex xs12 sm6 md4 text-center my-5>
        <v-card
        max-width="344"
        class="mx-auto"
        >
        <v-card-title>カレー屋さん</v-card-title>
        <v-card-text>カレーが一杯無料なんだよ</v-card-text>
        <v-card-actions>
          <v-btn text>もっとみる</v-btn>
        </v-card-actions>
        </v-card>
      </v-flex>

      <v-flex xs12 sm6 md4 text-center my-5>
        <v-card
        max-width="344"
        class="mx-auto"
        >
        <v-card-title>ロケット商会</v-card-title>
        <v-card-text>麻婆豆腐麺とご飯</v-card-text>
        <v-card-actions>
          <v-btn text>もっとみる</v-btn>
        </v-card-actions>
        </v-card>
      </v-flex>

      <v-flex xs12 sm6 md4 text-center my-5>
        <v-card
        max-width="344"
        class="mx-auto"
        >
        <v-card-title>侍</v-card-title>
        <v-card-text>美味しい家系ラーメン</v-card-text>
        <v-card-actions>
          <v-btn text>もっとみる</v-btn>
        </v-card-actions>
        </v-card>
      </v-flex>
    </v-layout>
    <!-- タイル終わり -->

    <!-- アコーディオン -->
    <!-- アコーディオン終わり -->







<v-expansion-panels>
    <v-expansion-panel
      v-for="(item,i) in 5"
      :key="i"
    >
      <v-expansion-panel-header>あこーでぃおん</v-expansion-panel-header>
      <v-expansion-panel-content>
        開くと説明文がでてくるよ。開くと説明文がでてくるよ。開くと説明文がでてくるよ。開くと説明文がでてくるよ。開くと説明文がでてくるよ。開くと説明文がでてくるよ。開くと説明文がでてくるよ。
      </v-expansion-panel-content>
    </v-expansion-panel>
  </v-expansion-panels>





    <v-layout wrap>
      <v-flex xs12 sm6 md4 text-center my-5><v-btn>押して</v-btn></v-flex>
      <v-flex xs12 sm6 md4 text-center my-5><v-btn>押して</v-btn></v-flex>
      <v-flex xs12 sm6 md4 text-center my-5><v-btn>押して</v-btn></v-flex>
    </v-layout>
    </v-container>
  </v-content>
</template>



<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'


export default {
  components: {
    Logo,
    VuetifyLogo,
  },
  data: () => ({
    drawer: null,
    // パンくずリスト
    items: [
      {
        text: 'Home',
        disabled: false,
        href: 'https://smoothe-777.com',
      },
      {
        text: '会社概要',
        disabled: false,
        href: 'https://smoothe-777.com',
      },
      {
        text: 'ご挨拶',
        disabled: true,
        href: 'https://smoothe-777.com',
      },
    ],
    // スライド
    colors: [
      'primary',
      'secondary',
      'yellow darken-2',
      'red',
      'orange'
    ],
  })
}
</script>



