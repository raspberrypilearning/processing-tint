Si vas a añadirle imágenes a tu proyecto, puedes usar `tint()` para cambiar el color de la imagen.

Pasar un color a `tint()` te permite cambiar los colores de cualquier imagen que dibujes después. Parecerá como si las imágenes tuviesen una luz que brilla del color que elegiste.

La función `no_tint()` desactiva `tint()` cuando hayas terminado de usarla.

Este ejemplo añade un `tint()` verde a ambas imágenes.

--- code ---
---
language: python
---

  tint(0, 255, 0) # Tinte verde 
  image(rocket, 50, 50, 100, 100) 
  image(planet, 50, 50, 300, 300)

--- /code ---

![El área de salida muestra un cohete y un planeta con ambos tintes](images/all_tint.png)

Este ejemplo añade un `tint()` verde a la primera imagen, luego lo quita usando `no_tint()` antes de dibujar la segunda imagen.

--- code ---
---
language: python
---

  tint(0, 255, 0) # Tinte verde 
  image(rocket, 50, 50, 100, 100) 
  no_tint() # Quitar tinte 
  image(planet, 50, 50, 300, 300)

--- /code ---

![El área de salida muestra un cohete coloreado y un planeta sin color](images/some_tint.png)

