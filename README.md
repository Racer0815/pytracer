# pytracer
a simple python raytracer implementation

---
## Features:
- Lambertian diffuse
- Metals with fuzziness
- The classic checkerboard floor texture
- Emissive materials
- Optional denoiser
- Live preview while rendering
- PPM file output
- Miserable performance (slow af) 

---
## Example renders:
To create your own renders: Modify samples, resolution, maxBounces and ambient occlusion in "src/main.py" and add objects to the scene by calling scene.addObject() and passing an object as a parameter.

<p align="center">
  <img height="380" src="https://github.com/magnusKue/pytracer/blob/main/results/final6.png">
  <img height="200" src="https://github.com/magnusKue/pytracer/blob/main/results/lights2.png">
  <img width="307" height="200"  src="https://github.com/magnusKue/pytracer/blob/main/results/fuzzSteps.png">
</p>

---
## Denoising:
To denoise a render: Run "denoiser/denoise.py", choose the input file in the first filedialogue and choose the output folder in the second.

<p align="center">
  <img height="220" src="https://github.com/magnusKue/pytracer/blob/b09168ebfc334fc42beac90bb375a7fe27ea9f3a/results/final1.png">
  <img height="220" src="https://github.com/magnusKue/pytracer/blob/b09168ebfc334fc42beac90bb375a7fe27ea9f3a/results/denoised/final1_denoised.png">
</p>

---
## Project structure
| Folder | content |
| --- | --- |
| results/ | All of my renders (even those from older more primitive versions of the raytracer) |
| └ results/denoised | denoised versions of some of the renders |
| └ results/fails | funny failed renders luckily i dont have many of those.. or sadly |
| output/ | This is where the resulting image file of a render is written to (also overwriting old ones!)|
| src/ | This is where the code is |
