If you are adding images to your project you can use `tint()` to change the colour of the image.

Passing a colour to `tint()` lets you change the colours of any image you draw after it. The images will look like they have a light of the colour you chose shining on them. 

The `no_tint()` function to turn `tint()` off when you’re finished with it.

This example adds a green `tint()` to both images. 

--- code ---
---
language: python
---

  tint(0, 200, 0) # Green tint
  image(planet, 50, 50, 300, 300)
  image(rocket, 50, 50, 100, 100) 

--- /code ---

![The output area showing a planet and rocket with both tinted](images/all-tint.png)

This example adds a green `tint()` to the first image then removes it using `no_tint()` before the second image is drawn. 

--- code ---
---
language: python
---

  tint(0, 200, 0) # Green tint
  image(planet, 50, 50, 300, 300)
  no_tint() # Remove tint
  image(rocket, 50, 50, 100, 100) 
--- /code ---

![The output area showing a tinted planet and a rocket without tint](images/some-tint.png)
