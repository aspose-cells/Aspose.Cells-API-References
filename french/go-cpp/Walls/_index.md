---
title: "Classe Walls"
linktitle: "Walls"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe Walls. Encapsule l'objet qui représente les murs dans Go."
type: docs
weight: 200
url: /fr/go-cpp/walls/
---

## Walls class

Encapsule l'objet qui représente les parois d'un graphique 3D.

```go

type Walls struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewWalls](./newwalls/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetCenterX](./getcenterx/) | Obtient la coordonnée x du coin inférieur gauche du centre du mur en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate(). |
| [GetCenterY](./getcentery/) | Obtient la coordonnée y du coin inférieur gauche du centre du mur en unités de 1/4000 de la hauteur du graphique après l'appel de la méthode Chart.Calculate(). |
| [GetWidth](./getwidth/) | Obtient la largeur de gauche à droite en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate(). |
| [GetDepth](./getdepth/) | Obtient la profondeur de l'avant à l'arrière en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate(). |
| [GetHeight](./getheight/) | Obtient la hauteur du haut vers le bas en unités de 1/4000 de la hauteur du graphique après l'appel de la méthode Chart.Calculate(). |
| [GetCenterXPx](./getcenterxpx/) | Obtient la coordonnée x du coin inférieur gauche du centre du mur en pixels après l'appel de la méthode Chart.Calculate(). |
| [GetCenterYPx](./getcenterypx/) | Obtient la coordonnée y du coin inférieur gauche du centre du mur en pixels après l'appel de la méthode Chart.Calculate(). |
| [GetWidthPx](./getwidthpx/) | Obtient la largeur de gauche à droite en pixels après l'appel de la méthode Chart.Calculate(). |
| [GetDepthPx](./getdepthpx/) | Obtient la profondeur de l'avant à l'arrière en pixels après l'appel de la méthode Chart.Calculate(). |
| [GetHeightPx](./getheightpx/) | Obtient la hauteur de haut en bas en unités de pixels après avoir appelé la méthode Chart.Calculate(). |
| [GetCubePointCount](./getcubepointcount/) | Obtient le nombre de points du cube après avoir appelé la méthode Chart.Calculate(). |
| [GetCubePointXPx](./getcubepointxpx/) | Obtient la coordonnée x du point d'apex du cube de murs après avoir appelé la méthode Chart.Calculate(). Le nombre de points d'apex du cube de murs est huit |
| [GetCubePointYPx](./getcubepointypx/) | Obtient la coordonnée y du point d'apex du cube de murs après avoir appelé la méthode Chart.Calculate(). Le nombre de points d'apex du cube de murs est huit. |
| [GetBackgroundColor](./getbackgroundcolor/) | Obtient ou définit la couleur d'arrière-plan de la zone. |
| [SetBackgroundColor](./setbackgroundcolor/) | Obtient ou définit la couleur d'arrière-plan de la zone. |
| [GetForegroundColor](./getforegroundcolor/) | Obtient ou définit la couleur de premier plan. |
| [SetForegroundColor](./setforegroundcolor/) | Obtient ou définit la couleur de premier plan. |
| [GetFormatting](./getformatting/) | Représente le formatage de la zone. |
| [SetFormatting](./setformatting/) | Représente le formatage de la zone. |
| [GetInvertIfNegative](./getinvertifnegative/) | Si la propriété est vraie et que la valeur du point du graphique est un nombre négatif, la couleur de premier plan et la couleur d'arrière-plan seront échangées. |
| [SetInvertIfNegative](./setinvertifnegative/) | Si la propriété est vraie et que la valeur du point du graphique est un nombre négatif, la couleur de premier plan et la couleur d'arrière-plan seront échangées. |
| [GetFillFormat](./getfillformat/) | Représente un objet FillFormat qui contient les propriétés de formatage de remplissage pour le graphique ou la forme spécifiés. |
| [GetTransparency](./gettransparency/) | Renvoie ou définit le degré de transparence de la zone sous forme d'une valeur allant de 0,0 (opaque) à 1,0 (transparent). |
| [SetTransparency](./settransparency/) | Renvoie ou définit le degré de transparence de la zone sous forme d'une valeur allant de 0,0 (opaque) à 1,0 (transparent). |
| [GetBorder](./getborder/) | Obtient ou définit la ligne de bordure. |
| [SetBorder](./setborder/) | Obtient ou définit la ligne de bordure. |
