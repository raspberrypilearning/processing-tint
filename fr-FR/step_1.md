Si tu ajoutes des images à ton projet, tu peux utiliser `tint()` pour changer la couleur de l'image.

Passer une couleur à `tint()` te permet de changer les couleurs de toute image que tu dessines après. Les images auront l'air d'avoir un peu de la couleur que tu as choisie qui brille sur elles.

La fonction `no_tint()` pour désactiver `tint()` lorsque tu en as terminé.

Cet exemple ajoute un `tint()` vert aux deux images.

--- code ---
---
language: python
---

  tint(0, 255, 0) # Teinte verte 
  image(rocket, 50, 50, 100, 100) 
  image(planet, 50, 50, 300, 300)

--- /code ---

![La zone de sortie montrant une fusée et une planète avec les deux teintées](images/all_tint.png)

Cet exemple ajoute un `tint()` vert à la première image puis le supprime en utilisant `no_tint()` avant que la deuxième image ne soit dessinée.

--- code ---
---
language: python
---

  tint(0, 255, 0) # Teinte verte 
  image(rocket, 50, 50, 100, 100) 
  no_tint() # Supprimer la teinte 
  image(planet, 50, 50, 300, 300)

--- /code ---

![La zone de sortie montrant une fusée teintée et une planète sans teinte](images/some_tint.png)

