---
title: "Classe ChartPoint"
linktitle: "ChartPoint"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe ChartPoint. Encapsule l'objet qui représente chartpoint en Go."
type: docs
weight: 200
url: /fr/go-cpp/chartpoint/
---

## ChartPoint class

Représente un point unique dans une série d'un graphique.

```go

type ChartPoint struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetExplosion](./getexplosion/) | La distance d'une tranche de pie ouverte du centre du pie chart est exprimée en pourcentage du diamètre du pie. |
| [SetExplosion](./setexplosion/) | La distance d'une tranche de pie ouverte du centre du pie chart est exprimée en pourcentage du diamètre du pie. |
| [GetShadow](./getshadow/) | Vrai si le chartpoint possède une ombre. |
| [SetShadow](./setshadow/) | Vrai si le chartpoint possède une ombre. |
| [GetBorder](./getborder/) | Obtient le Line</see>. |
| [GetArea](./getarea/) | Obtient le Area</see>. |
| [GetMarker](./getmarker/) | Obtient le Marker</see>. |
| [GetDataLabels](./getdatalabels/) | Renvoie un objet DataLabels qui représente l'étiquette de données associée à ce point de graphique. |
| [Get_YValue](./get_yvalue/) | Obtient ou définit la valeur Y du point du graphique. |
| [SetYValue](./setyvalue/) | Obtient ou définit la valeur Y du point du graphique. |
| [GetYValueType](./getyvaluetype/) | Obtient le type de valeur Y du point du graphique. |
| [GetXValue](./getxvalue/) | Obtient ou définit la valeur X du point du graphique. |
| [SetXValue](./setxvalue/) | Obtient ou définit la valeur X du point du graphique. |
| [GetXValueType](./getxvaluetype/) | Obtient le type de valeur X du point du graphique. |
| [GetShapeProperties](./getshapeproperties/) | Obtient l'objet ShapePropertyCollection qui contient les propriétés visuelles de forme du ChartPoint. |
| [IsInSecondaryPlot](./isinsecondaryplot/) | Obtient ou définit une valeur indiquant si ce point de données se trouve dans le deuxième secteur ou barre d'un graphique en secteurs ou en barres. |
| [SetIsInSecondaryPlot](./setisinsecondaryplot/) | Obtient ou définit une valeur indiquant si ce point de données se trouve dans le deuxième secteur ou barre d'un graphique en secteurs ou en barres. |
| [GetShapeX](./getshapex/) | Obtient la coordonnée x du coin supérieur gauche en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate(). |
| [GetShapeY](./getshapey/) | Obtient la coordonnée y du coin supérieur gauche en unités de 1/4000 de la hauteur du graphique après l'appel de la méthode Chart.Calculate(). |
| [GetShapeWidth](./getshapewidth/) | Obtient la largeur en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate(). |
| [GetShapeHeight](./getshapeheight/) | Obtient la hauteur en unités de 1/4000 de la hauteur du graphique après l'appel de la méthode Chart.Calculate(). |
| [GetShapeXPx](./getshapexpx/) | Obtient la coordonnée x du coin supérieur gauche en pixels après l'appel de la méthode Chart.Calculate(). |
| [GetShapeYPx](./getshapeypx/) | Obtient la coordonnée y du coin supérieur gauche en pixels après l'appel de la méthode Chart.Calculate(). |
| [GetShapeWidthPx](./getshapewidthpx/) | Obtient la largeur en pixels après l'appel de la méthode Chart.Calculate(). |
| [GetShapeHeightPx](./getshapeheightpx/) | Obtient la hauteur en pixels après l'appel de la méthode Chart.Calculate(). |
| [GetBorderWidthPx](./getborderwidthpx/) | Obtient la largeur de la bordure en pixels après l'appel de la méthode Chart.Calculate(). |
| [GetRadiusPx](./getradiuspx/) | Obtient le rayon de la bulle, du secteur ou du beignet en pixels après l'appel de la méthode Chart.Calculate(). |
| [GetDoughnutInnerRadius](./getdoughnutinnerradius/) | Obtient le rayon interne de la tranche de beignet en pixels après l'appel de la méthode Chart.Calculate(). S'applique au graphique Doughnut. |
| [GetStartAngle](./getstartangle/) | Obtient l'angle de départ de la section du secteur, mesuré en degrés dans le sens des aiguilles d'une montre à partir de l'axe x après l'appel de la méthode Chart.Calculate(). S'applique au graphique Pie. |
| [GetEndAngle](./getendangle/) | Obtient l'angle de fin de la section du secteur, mesuré en degrés dans le sens des aiguilles d'une montre à partir de l'axe x après l'appel de la méthode Chart.Calculate(). S'applique au graphique Pie. |
| [GetArcStartPointXPx](./getarcstartpointxpx/) | Obtient la coordonnée x du point de départ de la section du secteur après l'appel de la méthode Chart.Calculate(). S'applique aux graphiques Pie et Doughnut. |
| [GetArcStartPointYPx](./getarcstartpointypx/) | Obtient la coordonnée y du point de départ de la section du secteur après l'appel de la méthode Chart.Calculate(). S'applique aux graphiques Pie et Doughnut. |
| [GetArcEndPointXPx](./getarcendpointxpx/) | Obtient la coordonnée x du point d'arrivée de la section du secteur après l'appel de la méthode Chart.Calculate(). S'applique aux graphiques Pie et Doughnut. |
| [GetArcEndPointYPx](./getarcendpointypx/) | Obtient la coordonnée y du point d'arrivée de la section du secteur après l'appel de la méthode Chart.Calculate(). S'applique aux graphiques Pie et Doughnut. |
| [GetInnerArcStartPointXPx](./getinnerarcstartpointxpx/) | Obtient la coordonnée x du point de départ de la section du secteur après l'appel de la méthode Chart.Calculate(). S'applique au graphique Doughnut. |
| [GetInnerArcStartPointYPx](./getinnerarcstartpointypx/) | Obtient la coordonnée y du point de départ de la section du secteur après l'appel de la méthode Chart.Calculate(). S'applique au graphique Doughnut. |
| [GetInnerArcEndPointXPx](./getinnerarcendpointxpx/) | Obtient la coordonnée x du point final de la section du secteur après avoir appelé la méthode Chart.Calculate(). S'applique aux graphiques en anneau. |
| [GetInnerArcEndPointYPx](./getinnerarcendpointypx/) | Obtient la coordonnée y du point final de la section du secteur après avoir appelé la méthode Chart.Calculate(). S'applique au graphique en anneau. |
| [GetTopPointCount](./gettoppointcount/) | Obtient le nombre de points supérieurs après avoir appelé la méthode Chart.Calculate(). |
| [GetTopPointXPx](./gettoppointxpx/) | Obtient la coordonnée x du point supérieur de la forme après avoir appelé la méthode Chart.Calculate(). S'applique aux graphiques 3D : Column3D, Bar3D, Cone, Cylinder, Pyramid et Area3D. |
| [GetTopPointYPx](./gettoppointypx/) | Obtient la coordonnée y du point supérieur de la forme après avoir appelé la méthode Chart.Calculate(). S'applique aux graphiques 3D : Column3D, Bar3D, Cone, Cylinder, Pyramid, et Area3D. |
| [GetBottomPointCount](./getbottompointcount/) | Obtient le nombre de points inférieurs après avoir appelé la méthode Chart.Calculate(). |
| [GetBottomPointXPx](./getbottompointxpx/) | Obtient la coordonnée x du point inférieur de la forme après avoir appelé la méthode Chart.Calculate(). S'applique aux graphiques 3D : Column3D, Bar3D, Cone, Cylinder, Pyramid. |
| [GetBottomPointYPx](./getbottompointypx/) | Obtient la coordonnée y du point inférieur de la forme après avoir appelé la méthode Chart.Calculate(). S'applique aux graphiques 3D : Column3D, Bar3D, Cone, Cylinder, Pyramid. |
| [GetOnCategoryAxisPointCount](./getoncategoryaxispointcount/) | Obtient le nombre de points sur l'axe des catégories après avoir appelé la méthode Chart.Calculate(). S'applique uniquement aux graphiques de zone. |
| [GetOnCategoryAxisPointXPx](./getoncategoryaxispointxpx/) | Obtient la coordonnée x du point sur l'axe des catégories après avoir appelé la méthode Chart.Calculate(). S'applique uniquement au graphique de zone. |
| [GetOnCategoryAxisPointYPx](./getoncategoryaxispointypx/) | Obtient la coordonnée y du point sur l'axe des catégories après avoir appelé la méthode Chart.Calculate(). S'applique uniquement au graphique de zone. |
