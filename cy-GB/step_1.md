Os ydych chi'n ychwanegu delweddau at eich prosiect, fe allwch chi ddefnyddio`tint()` i newid lliw'r ddelwedd.

Mae pasio lliw i `tint()` yn gadael i chi newid lliw unrhyw ddelwedd rydych chi'n ei llunio ar ei ôl. Bydd y delweddau'n edrych fel bod ganddyn nhw olau o'r lliw o'ch dewis yn disgleirio arnyn nhw.

Y swyddogaeth `no_tint()` i ddiffodd `tint()` pan na fyddwch chi ei angen mwyach.

Mae'r enghraifft hon yn ychwanegu arlliw gwyrdd at y ddwy ddelwedd.

--- code ---
---
language: python
---

  tint(0, 255, 0) # Arlliw gwyrdd 
  image(roced, 50, 50, 100, 100) 
  image(planed, 50, 50, 300, 300)

--- /code ---

![Yr ardal allbwn yn dangos roced a phlaned, a'r ddau ag arlliw](images/all_tint.png)

Mae'r enghraifft hon yn ychwanegu arlliw gwyrdd i'r ddelwedd gyntaf ac yna'n ei dynnu gyda `no_tint()` cyn llunio'r ail ddelwedd.

--- code ---
---
language: python
---

  tint(0, 255, 0) # Arlliw gwyrdd 
  image(roced, 50, 50, 100, 100) 
  no_tint() # Tynnu arlliw 
  image(planed, 50, 50, 300, 300)

--- /code ---

![Yr ardal allbwn yn dangos roced ag arlliw, a phlaned heb arlliw](images/some_tint.png)

