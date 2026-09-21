# カキトリ 筆順データ

小学校配当漢字1026字の筆順データ。[KanjiVG](http://kanjivg.tagaini.net) を加工したもの。

## ライセンス

[Creative Commons Attribution-Share Alike 3.0](http://creativecommons.org/licenses/by-sa/3.0/)

- 原典：KanjiVG（Copyright (C) 2009-2013 Ulrich Apel） http://kanjivg.tagaini.net
- 原典の版：20250816
- 公開先：https://github.com/erosegalaxy/kakitori-stroke-data
- このデータも同じ CC BY-SA 3.0 で配布する。

## 改変した内容

原典からの変更は次のとおり。字形そのものは変えていない。

1. 小学校配当の1026字だけを取り出した。
2. SVG のパス（曲線）を折れ線に直し、1画あたり 32 点に等間隔で取り直した。
3. 座標を 109×109 の座標系から 0〜1 に変換した（縦横比は保持。はみ出しは切り詰めていない）。
4. 1字1ファイルの JSON にした。画の種類（KanjiVG の `kvg:type`）はそのまま残している。

## 形式

```json
{
  "kanji": "右",
  "codePoint": "U+53F3",
  "gradeLevel": 1,
  "strokeCount": 5,
  "source": { "dataset": "KanjiVG", "version": "20250816", "license": "CC BY-SA 3.0" },
  "strokes": [ { "type": "㇒", "points": [[0.4908, 0.1972], ...] } ]
}
```

`strokes` は筆順どおりに並ぶ。`points` は書き始めから書き終わりの順。

生成日：2026-09-21
