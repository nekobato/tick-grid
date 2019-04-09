<template>
  <div id="app">
    <TickScroll tick="10" class="tick">
      <h1>Title</h1>
      <nav>
        <ul>
          <li>menu1</li>
          <li>menu2</li>
          <li>menu3</li>
          <li>menu4</li>
        </ul>
      </nav>
      <p>
        昨日、近所の吉野家行ったんです。吉野家。
        <br>そしたらなんか人がめちゃくちゃいっぱいで座れないんです。
        <br>で、よく見たらなんか垂れ幕下がってて、１５０円引き、とか書いてあるんです。
        <br>もうね、アホかと。馬鹿かと。
        <br>お前らな、１５０円引き如きで普段来てない吉野家に来てんじゃねーよ、ボケが。
        <br>１５０円だよ、１５０円。
        <br>なんか親子連れとかもいるし。一家４人で吉野家か。おめでてーな。
        <br>よーしパパ特盛頼んじゃうぞー、とか言ってるの。もう見てらんない。
        <br>お前らな、１５０円やるからその席空けろと。
        <br>吉野家ってのはな、もっと殺伐としてるべきなんだよ。
        <br>Ｕの字テーブルの向かいに座った奴といつ喧嘩が始まってもおかしくない、
        <br>刺すか刺されるか、そんな雰囲気がいいんじゃねーか。女子供は、すっこんでろ。
        <br>で、やっと座れたかと思ったら、隣の奴が、大盛つゆだくで、とか言ってるんです。
        <br>そこでまたぶち切れですよ。
        <br>あのな、つゆだくなんてきょうび流行んねーんだよ。ボケが。
        <br>得意げな顔して何が、つゆだくで、だ。
        <br>お前は本当につゆだくを食いたいのかと問いたい。問い詰めたい。小１時間問い詰めたい。
        <br>お前、つゆだくって言いたいだけちゃうんかと。
        <br>吉野家通の俺から言わせてもらえば今、吉野家通の間での最新流行はやっぱり、
        <br>ねぎだく、これだね。
        <br>大盛りねぎだくギョク。これが通の頼み方。
        <br>ねぎだくってのはねぎが多めに入ってる。そん代わり肉が少なめ。これ。
        <br>で、それに大盛りギョク（玉子）。これ最強。
        <br>しかしこれを頼むと次から店員にマークされるという危険も伴う、諸刃の剣。
        <br>素人にはお薦め出来ない。
        <br>まあお前らド素人は、牛鮭定食でも食ってなさいってこった。
      </p>
    </TickScroll>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import TickScroll from './components/TickScroll.vue';

export default Vue.extend({
  name: 'app',
  components: {
    TickScroll,
  },
});
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.tick {
  height: 200px;
}
</style>
