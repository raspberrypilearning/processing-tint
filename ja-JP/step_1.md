プロジェクトに画像を使っている場合、 `tint()` を使って画像の色を変更できます。

`tint()`に色指定を渡すと、その後に描画する画像の色を変更できます。 画像は、選択した色のライトで照らしているように見えます。

`no_tint()` 関数は、`tint()` を使い終わった後に オフにします。

この例では、両方の画像に緑の `tint()` （色合い）を追加しています。

--- code ---
---
language: python
---

  tint(0, 255, 0) # 緑の色合い 
  image(rocket, 50, 50, 100, 100) 
  image(planet, 50, 50, 300, 300)

--- /code ---

![両方の色合いが変更されたロケットと惑星を描いた出力領域](images/all_tint.png)

この例では、最初の画像に緑の `tint()` を追加し、2番目の画像が描画される前に `no_tint()` を使用してそれを削除しています。

--- code ---
---
language: python
---

  tint(0, 255, 0) # 緑の色合い 
  image(rocket, 50, 50, 100, 100) 
  no_tint() # 色合いを削除 
  image(planet, 50, 50, 300, 300)

--- /code ---

![色合いが変更されたロケットと変更されていない惑星を描いた出力領域](images/some_tint.png)

