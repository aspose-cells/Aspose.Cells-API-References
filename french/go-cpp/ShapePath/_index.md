---
title: "ShapePath Class"
linktitle: "ShapePath"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "ShapePath class. Encapsule l'objet qui représente shapepath en Go."
type: docs
weight: 200
url: /fr/go-cpp/shapepath/
---

## ShapePath class

Représente un chemin de création composé d'une série de déplacements, de lignes et de courbes qui, une fois combinés, formeront une forme géométrique.

```go

type ShapePath struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewShapePath](./newshapepath/) | Initialise une nouvelle instance de la classe ShapePath. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetPathSegments](./getpathsegments/) | Obtient la liste ShapeSegmentPathCollection. |
| [GetWidthPixel](./getwidthpixel/) | Obtient la largeur de ce chemin en unités de pixels. |
| [SetWidthPixel](./setwidthpixel/) | Obtient la largeur de ce chemin en unités de pixels. |
| [GetHeightPixel](./getheightpixel/) | Obtient la hauteur de ce chemin en unités de pixels. |
| [SetHeightPixel](./setheightpixel/) | Obtient la hauteur de ce chemin en unités de pixels. |
| [MoveTo](./moveto/) | Démarre une nouvelle figure à partir du point spécifié sans fermer la figure actuelle. Tous les points suivants ajoutés au chemin sont ajoutés à cette nouvelle figure. Unité : Pixel. |
| [LineTo](./lineto/) | Ajoute un segment de ligne à la figure actuelle. Le point de départ est le point final de la figure actuelle. Unité : Pixel. |
| [CubicBezierTo](./cubicbezierto/) | Ajoute une courbe cubique de Bézier à la figure actuelle. Le point de départ est le point final de la figure actuelle. Unité : Pixel. |
| [ArcTo](./arcto/) | Ajoute un arc elliptique à la figure actuelle. Le point de départ est le point final de la figure actuelle. |
| [Close](./close/) | Ferme la figure actuelle et démarre une nouvelle figure. Si la figure actuelle contient une séquence de lignes et de courbes connectées, la méthode ferme la boucle en reliant une ligne du point final au point de départ. |
