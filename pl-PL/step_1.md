Jeśli dodajesz obrazy do swojego projektu, możesz użyć `tint()`, aby zmienić kolor obrazu.

Przekazanie koloru do `tint()` pozwala zmienić kolory dowolnego obrazu, który narysujesz po nim. Obrazy będą wyglądać tak, jakby świeciło na nich światło w wybranym przez Ciebie kolorze.

Funkcja `no_tint()` wyłącza funkcję `tint()`, kiedy skończysz z nią pracować.

Ten przykład dodaje zielony `tint()` do obu obrazów.

--- code ---
---
language: python
---

  tint(0, 255, 0) # Green tint image(rocket, 50, 50, 100, 100) image(planet, 50, 50, 300, 300)

--- /code ---

![Wyjściowy obraz przedstawiający zabarwioną zarówno rakietę, jak i planetę](images/all_tint.png)

Ten przykład dodaje zielony `tint()` do pierwszego obrazu, a następnie usuwa go za pomocą `no_tint()` przed narysowaniem drugiego obrazu.

--- code ---
---
language: python
---

  tint(0, 255, 0) # Green tint image(rocket, 50, 50, 100, 100) no_tint() # Remove tint image(planet, 50, 50, 300, 300)

--- /code ---

![Wyjściowy obraz przedstawiający zabarwioną rakietę i planetę bez zabarwienia](images/some_tint.png)

