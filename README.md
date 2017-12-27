# itachoco sketch guideline

1. [Naming Rules](#naming-rules)
1. [Layers](#layers)
1. [Symbols](#symbols)
1. [Export](#export)

## 1. Naming Rules

### Pages & Artboards & Layers & Symbols

大文字から始める英単語で記載する。  
単語と単語の区切りは半角スペースを空け、アンダースコアでつなげたりしない。  
キャメルケースも使わない。

#### ex) Artboards

```
{{ Page Name }} - {{ 画面名とか状態とかパターンとか }} - {{ 画面名とか状態とかパターンとか }}
```

- Product Detail
- Product Detail - ◯◯◯◯
- Product Detail - ◯◯◯◯ - Empty
- Product Detail - ◯◯◯◯ - ◯◯のとき
- Product Detail - Book
- Product Detail - CD

#### ex) Layers

```
{{ Element Name }} - {{ 画面名とか状態とかパターンとか }} - {{ 画面名とか状態とかパターンとか }}
```

- Table Cell
- Table Cell - ◯◯◯◯
- Table Cell - Book
- Table Cell - CD

#### Similar name

- Arrow
  - Chevron
- Border
  - Divider
  - Separator
  - Key Line
- Background
  - Rectangle


## 2. Layers

OS標準UIは1番上にする（成立しない場合はこの限りではない）  
わかりやすい粒度でグルーピングする。  
Artboard直下とSymbol配下の重なり順は見た目に準じる。（上にあるものから下にあるものへ向かって重なり順）

### Element Name

- Section
- Navigation
- Title
- Item
- Image
- Text
- Label
- Button
- Icon
- Table Cell


## 3. Symbols

適切な粒度でスラッシュ区切りとハイフン区切りのルールを決める（プロジェクトにあわせよう）  
ちょーーー大規模だったらスラッシュが多くなりそう。  
ネストし過ぎにならないように注意。

### Element Name

- *iOS
- *Android
- Component
- Button
- Icon
- Label
- Form

```
ex)
Icon/Like - Medium - Fill
Icon/Like - Large - Outline
Button/Primary - Large
Button/Secondary - Medium
Button/Secondary - W100
Button/Secondary - W200 - Orange
```

## 4. Export

接続はアンダースコアに統一する。すべて小文字。

```
{{ Prefix }}_{{ View Name }}_{{ Name }}_{{ Size }}_{{ 色 }}_{{ 形状 }}_{{ 状態 }}
```

### Prefix

Prefixは以下の省略形式から採用する。

- ic_
- img_
- btn_
- bg_

### Suffix

Suffixは省略しない。状態・色・サイズなど。

#### サイズ

- _xsmall
- _small
- _medium
- _large
- _xlarge
- _40

#### 色

- _white
- _black
- _orange
- _blue
- _gray

#### 形状

- _fill
- _outline

#### 状態

- _on (Toggleのとき)
- _off (Toggleのとき)
- _disable


# Changelog

- 2017.12.27 v0.1


# Author

[@wataame](https://twitter.com/wataame)
[@urakey](https://twitter.com/urakey)
