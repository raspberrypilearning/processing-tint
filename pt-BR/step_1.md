Se você estiver adicionando imagens ao seu projeto, poderá usar `tint()` para alterar a cor da imagem.

Passar uma cor para `tint()` permite você alterar as cores de qualquer imagem desenhada depois dela. As imagens parecerão ter uma luz da cor que você escolheu brilhando nelas.

A função `no_tint()` para desativar `tint()` quando você terminar com ela.

Este exemplo adiciona uma `tint()` verde a ambas as imagens.

--- code ---
---
language: python
---

  tint(0, 255, 0) # Coloração verde image(foguete, 50, 50, 100, 100) image(planeta, 50, 50, 300, 300)

--- /code ---

![A área de saída mostrando um foguete e um planeta, ambos coloridos](images/all_tint.png)

Este exemplo adiciona um `tint()` verde à primeira imagem e o remove usando `no_tint()` antes que a segunda imagem seja desenhada.

--- code ---
---
language: python
---

  tint(0, 255, 0) # Coloração verde image(foguete, 50, 50, 100, 100) no_tint() # Remove coloração verde image(planeta, 50, 50, 300, 300)

--- /code ---

![A área de saída mostrando um foguete colorido e um planeta sem coloração](images/some_tint.png)

