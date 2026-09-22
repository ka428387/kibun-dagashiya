# きぶん駄菓子屋

いまの気分と予算を選ぶと、店主が愛する駄菓子をひとこと付きでおすすめするページ。

## 駄菓子を追加・編集するには

`index.html` の中の `<script type="application/json" id="catalog">` にあるリストを書き換えます。1品はこんな形です。

```json
{"id":"big-katsu","name":"ビッグカツ","maker":"すぐる","price":40,"tastes":["しょっぱい","ソース"],"moods":["hungry","otsumami"],"love":5,"comment":"駄菓子界のメインディッシュ。"}
```

- `moods` に入れられる気分: `tired` つかれた / `sweet` あまいの / `salty` しょっぱいの / `sour` すっぱさ / `hungry` 小腹 / `focus` 作業のおとも / `otsumami` 晩酌 / `share` みんなで分けたい / `luck` 運だめし / `nostalgic` なつかしい
- `love` は偏愛度（1〜5）。高いほどおすすめに出やすくなります
- `"sample":true` が付いている品は、ひとことが見本の文章です。書き換えたら消してください
