# Procedural generation using noise functions

## 1) General

This is a Unity project without a standalone executable.<br>
The project can be directly added to Unity, native version being 2020.1.2f1.<br>
The powerpoint presentation that was made for this showcase can be downloaded [here](https://www.dropbox.com/s/wh8s19lj9wke2gn/Noise-and-what-it-looks-like.pptx?dl=0).

## 2) Gradient noise

The main showcase of gradient (simplex) noise and layering is found in `GradientNoiseScene.unity`.<br>
The Terrain gameobject holds the `GradientNoiseTerrainGenerator.cs`.
- All values used in calculations can be accessed from the inspector.
- The original presentation primarily covered Perlin noise, of which Simplex noise is a successor that improves pattern angle distribution. In the spirit of progress, this tech demo has been updated to showcase Simplex noise. Both noises fall under the more-general category of gradient noise.


## 3) Voronoi Diagrams/Worley noise

The main showcase of voronoi diagrams is found in `VoronoiScene.unity`.<br>
The Terrain gameobject holds `VoronoiTerrainGenerator.cs` which creates the shown terrain.<br>
The `exampleSprite` object (child object of `Main Camera`) holds `VoronoiDiagram.cs` which creates the initial voronoi diagram shown.
- All values used in calculations can be accessed from the inspector.


## 4) Blue noise

The main showcase of blue noise and layering it with gradient (simplex) and voronoi is found in `VoronoiScene.unity`.<br>
The Terrain gameobject holds `BlueNoiseSprite.cs` which creates the assets placed by the noise function.
- All values used in calculations can be accessed from the inspector.


## 4) Sources, references and helpful links

General:
- [https://www.ronja-tutorials.com/](https://www.ronja-tutorials.com/)

Gradient noise:
- [https://en.wikipedia.org/wiki/Gradient_noise](https://en.wikipedia.org/wiki/Gradient_noise)
- [https://weber.itn.liu.se/~stegu/simplexnoise/simplexnoise.pdf](https://weber.itn.liu.se/~stegu/simplexnoise/simplexnoise.pdf)

Worley noise:
- [https://thebookofshaders.com/12/](https://thebookofshaders.com/12/)
- [https://en.wikipedia.org/wiki/Voronoi_diagram](https://en.wikipedia.org/wiki/Voronoi_diagram)
- [https://](https://github.com/jushii/WorleyNoise)[github.com](https://github.com/jushii/WorleyNoise)[/](https://github.com/jushii/WorleyNoise)[jushii](https://github.com/jushii/WorleyNoise)[/](https://github.com/jushii/WorleyNoise)[WorleyNoise](https://github.com/jushii/WorleyNoise)

Blue noise:
- [https://de.wikipedia.org/wiki/Hard-core-Prozess](https://de.wikipedia.org/wiki/Hard-core-Prozess)
