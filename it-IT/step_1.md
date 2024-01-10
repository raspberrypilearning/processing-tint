Se stai aggiungendo delle immagini al tuo progetto, puoi usare `tint()` per cambiare il colore dell'immagine.

Passare un colore a `tint()` ti consente di modificare i colori di qualsiasi immagine che disegni dopo questo comando. Le immagini appariranno come se ci fosse una luce, del colore che hai scelto, che le illumina.

La funzione `no_tint()` serve per disattivare `tint()` quando non ti serve più.

Questo esempio usa `tint()` per aggiungere una tinta verde a entrambe le immagini.

--- code ---
---
language: python
---

  tint(0, 255, 0) # Tinta verde
  image(rocket, 50, 50, 100, 100)
  image(planet, 50, 50, 300, 300)

--- /code ---

![L'area di output mostra un razzo e un pianeta, entrambi colorati](images/all_tint.png)

Questo esempio usa `tint()` per aggiungere una tinta verde alla prima immagine, quindi usa `no_tint()` per rimuovere l'effetto prima che venga disegnata la seconda immagine.

--- code ---
---
language: python
---

  tint(0, 255, 0) # Tinta verde
  image(rocket, 50, 50, 100, 100)
  no_tint() # Disattiva effetto tinta
  image(planet, 50, 50, 300, 300)
  
--- /code ---

![L'area di output mostra un razzo con l'effetto tinta applicato e un pianeta senza effetto applicato](images/some_tint.png)

