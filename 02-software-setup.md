---
layout: default
title: 02.ソフトウェアセットアップ
nav_order: 3
---

# 02.ソフトウェアセットアップ
<br><br>

<img src="assets/02-1.jpg" width="640" alt="hi" class="inline"/><br>
<br>

ubuntuの左側メニューアイコンから**ターミナル（Terminal）**を開き、**"fab"**と入力してEnterキーを押します。<br>
そうすると**「Fabmodule」**というソフトが起動します。<br>
<br>
<br>
<br>

<img src="assets/02-2.jpg" width="640" alt="hi" class="inline"/><br>
<br>

* **from input format:** Meshs(.stl)
* **to output process:** Roland MDX-20 mill(.rml)

上記のように設定したら**「make_stl_rml」**ボタンをクリックします。<br>
<br>
<br>
<br>

<img src="assets/02-3.jpg" width="640" alt="hi" class="inline"/><br>

ウィンドウ左側の**「load.stl」**をクリックし、<br>
加工したいstlデータを選択して**「Open」**ボタンをクリックします。<br>
加工したいデータのサイズに間違いがないか確認したら、**「make.png」**をクリックします。<br>
<br>
<br>
<br>

<img src="assets/02-4.jpg" width="640" alt="hi" class="inline"/><br>
<br>

ウィンドウ上部のプルダウンメニューから**"mm, 1/8, wax, rough"**を選択します。<br>
更に、ウィンドウ下部の各種設定欄に任意の数値を入力します。<br>
（使用する材料によって、数値は変える必要があります。）<br>
<br>

**左側**<br>

* **stl units(mm/unit)：**STLファイルの単位（mmの場合は"1"）
* **png resolution(pixcels/mm)：**PNGの解像度。基本的にいじらない。
* **side：**STLファイルのどの面を削るのか。基本的にいじらない。

<br>

**右側**<br>

* **type：** 削り方の設定。まずはラフカットを行うので、ここでは"3D rough"を選択します。
* **diameter(mm)：**使用するエンドミルの刃の直径。
* **overlab(0-1)：**ツールパスをどれくらい重ねるか。<br>
1に近づくほど、時間はかかるが滑らかな仕上がりになります。
* **top intensity(0-1)：**不明。いじらなくてOK。
* **bot intensity(0-1)：**不明。いじらなくてOK。
* **offsets(-1 to fill)：**3D切削の場合は"-1"に設定します。
* **error(pixels)：**不明。いじらなくてOK。
* **top z(mm)：**切削範囲の上限高さ。
* **bot z(mm)：**切削範囲の下限高さ。
* **cut depth(mm)：**各階層の削る厚さ。薄いほど切削時間は増えますが、マシンへの負荷が減ります。

<br>
すべての設定が完了したら**「make.path」**ボタンをクリックします。<br>
そうすると、実際の加工パス（エンドミルの動くライン）が表示されます。<br>
<br>
<br>
<br>
<br>
<br>
<br>
