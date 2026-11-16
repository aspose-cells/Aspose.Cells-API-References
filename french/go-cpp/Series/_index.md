---
title: "Classe Series"
linktitle: "Series"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe Series. Encapsule l'objet qui représente series en Go."
type: docs
weight: 200
url: /fr/go-cpp/series/
---

## Series class

Encapsule l'objet qui représente une série de données unique dans un graphique.

```go

type Series struct  {
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
| [IsFiltered](./isfiltered/) | Indique si la série est sélectionnée ou filtrée. True indique que cette série est filtrée, et elle ne sera pas affichée sur le graphique. |
| [SetIsFiltered](./setisfiltered/) | Indique si la série est sélectionnée ou filtrée. True indique que cette série est filtrée, et elle ne sera pas affichée sur le graphique. |
| [GetLayoutProperties](./getlayoutproperties/) | Représente les propriétés de la mise en page. |
| [Move](./move/) | Déplace la série vers le haut ou vers le bas. |
| [GetPoints](./getpoints/) | Obtient la collection de points d'une série dans un graphique. |
| [GetArea](./getarea/) | Représente la zone d'arrière-plan de l'objet Series. |
| [GetBorder](./getborder/) | Représente la bordure d'un objet Series. |
| [GetName](./getname/) | Obtient ou définit le nom de la série de données. |
| [SetName](./setname/) | Obtient ou définit le nom de la série de données. |
| [GetDisplayName](./getdisplayname/) | Obtient le nom de la série affiché sur le graphique. |
| [GetCountOfDataValues](./getcountofdatavalues/) | Obtient le nombre de valeurs de données. |
| [IsVerticalValues](./isverticalvalues/) | Indique si la source de données est verticale. |
| [GetValues](./getvalues/) | Représente les valeurs Y de cette série de graphique. |
| [SetValues](./setvalues/) | Représente les valeurs Y de cette série de graphique. |
| [GetPointValues](./getpointvalues/) | Obtient les valeurs réelles utilisées pour tracer chaque point de cette série dans le graphique. |
| [GetCategoryValues](./getcategoryvalues/) | Obtient les valeurs de catégorie réelles utilisées pour tracer chaque point de cette série dans le graphique. |
| [GetValuesFormatCode](./getvaluesformatcode/) | Représente le code de format de la NumberList Values. |
| [SetValuesFormatCode](./setvaluesformatcode/) | Représente le code de format de la NumberList Values. |
| [GetXValuesFormatCode](./getxvaluesformatcode/) | Représente le code de format de la NumberList des X Values. |
| [SetXValuesFormatCode](./setxvaluesformatcode/) | Représente le code de format de la NumberList des X Values. |
| [GetXValues](./getxvalues/) | Représente les valeurs X de cette série de graphique. |
| [SetXValues](./setxvalues/) | Représente les valeurs X de cette série de graphique. |
| [GetBubbleSizes](./getbubblesizes/) | Obtient ou définit les valeurs de taille des bulles de la série de graphique. |
| [SetBubbleSizes](./setbubblesizes/) | Obtient ou définit les valeurs de taille des bulles de la série de graphique. |
| [GetTrendLines](./gettrendlines/) | Renvoie toutes les lignes de tendance de cette série. |
| [GetSmooth](./getsmooth/) | Représente le lissage de courbe. True si le lissage de courbe est activé pour le graphique en ligne ou le graphique en nuage de points. S'applique uniquement aux graphiques en ligne et aux graphiques en nuage de points avec lignes. |
| [SetSmooth](./setsmooth/) | Représente le lissage de courbe. True si le lissage de courbe est activé pour le graphique en ligne ou le graphique en nuage de points. S'applique uniquement aux graphiques en ligne et aux graphiques en nuage de points avec lignes. |
| [GetShadow](./getshadow/) | True si la série a une ombre. |
| [SetShadow](./setshadow/) | True si la série a une ombre. |
| [GetHas3DEffect](./gethas3deffect/) | True si la série a une apparence tridimensionnelle. |
| [SetHas3DEffect](./sethas3deffect/) | True si la série a une apparence tridimensionnelle. |
| [GetBar3DShapeType](./getbar3dshapetype/) | Obtient ou définit le type de forme 3D utilisé avec le graphique à barres ou à colonnes 3-D. |
| [SetBar3DShapeType](./setbar3dshapetype/) | Obtient ou définit le type de forme 3D utilisé avec le graphique à barres ou à colonnes 3-D. |
| [GetDataLabels](./getdatalabels/) | Représente l'objet DataLabels pour le ASeries spécifié. |
| [GetType](./gettype/) | Obtient ou définit le type d'une série de données. |
| [SetType](./settype/) | Obtient ou définit le type d'une série de données. |
| [GetMarker](./getmarker/) | Obtient le Marker</see>. |
| [GetPlotOnSecondAxis](./getplotonsecondaxis/) | Indique si cette série est tracée sur le deuxième axe des valeurs. |
| [SetPlotOnSecondAxis](./setplotonsecondaxis/) | Indique si cette série est tracée sur le deuxième axe des valeurs. |
| [GetXErrorBar](./getxerrorbar/) | Représente la barre d'erreur en direction X de la série. |
| [GetYErrorBar](./getyerrorbar/) | Représente la barre d'erreur en direction Y de la série. |
| [GetHasHiLoLines](./gethashilolines/) | True si le graphique en ligne possède des lignes haut-bas. S'applique uniquement aux graphiques en ligne. |
| [SetHasHiLoLines](./sethashilolines/) | True si le graphique en ligne possède des lignes haut-bas. S'applique uniquement aux graphiques en ligne. |
| [GetHiLoLines](./gethilolines/) | Renvoie un objet HiLoLines qui représente les lignes haut-bas pour une série sur un graphique en ligne. S'applique uniquement aux graphiques en ligne. |
| [GetHasSeriesLines](./gethasserieslines/) | Vrai si un stacked column chart ou un bar chart possède des series lines ou si un Pie of Pie chart ou un Bar of Pie chart possède des connector lines entre les deux sections. S'applique uniquement aux stacked column charts, bar charts, Pie of Pie charts, ou Bar of Pie charts. |
| [SetHasSeriesLines](./sethasserieslines/) | Vrai si un stacked column chart ou un bar chart possède des series lines ou si un Pie of Pie chart ou un Bar of Pie chart possède des connector lines entre les deux sections. S'applique uniquement aux stacked column charts, bar charts, Pie of Pie charts, ou Bar of Pie charts. |
| [GetSeriesLines](./getserieslines/) | Renvoie un objet SeriesLines qui représente les series lines pour un stacked bar chart ou un stacked column chart. S'applique uniquement aux stacked bar et stacked column charts. |
| [GetHasDropLines](./gethasdroplines/) | Vrai si le graphique possède des drop lines. S'applique uniquement aux line chart ou aux area charts. |
| [SetHasDropLines](./sethasdroplines/) | Vrai si le graphique possède des drop lines. S'applique uniquement aux line chart ou aux area charts. |
| [GetDropLines](./getdroplines/) | Renvoie un objet Line qui représente les drop lines pour une série sur le line chart ou le area chart. S'applique uniquement aux line charts ou aux area charts. |
| [GetHasUpDownBars](./gethasupdownbars/) | Vrai si un line chart possède des up bars et down bars. S'applique uniquement aux line charts. |
| [SetHasUpDownBars](./sethasupdownbars/) | Vrai si un line chart possède des up bars et down bars. S'applique uniquement aux line charts. |
| [GetUpBars](./getupbars/) | Renvoie un objet DropBars qui représente les up bars sur un line chart. S'applique uniquement aux line charts. |
| [GetDownBars](./getdownbars/) | Renvoie un objet DropBars qui représente les down bars sur un line chart. S'applique uniquement aux line charts. |
| [IsColorVaried](./iscolorvaried/) | Représente si la couleur des points est variée. Le graphique doit contenir une seule série ou ce graphique est un pie chart. |
| [SetIsColorVaried](./setiscolorvaried/) | Représente si la couleur des points est variée. Le graphique doit contenir une seule série ou ce graphique est un pie chart. |
| [GetGapWidth](./getgapwidth/) | Renvoie ou définit l'espace entre les groupes de barres ou de colonnes, en pourcentage de la largeur de la barre ou de la colonne. La valeur de cette propriété doit être comprise entre 0 et 500. |
| [SetGapWidth](./setgapwidth/) | Renvoie ou définit l'espace entre les groupes de barres ou de colonnes, en pourcentage de la largeur de la barre ou de la colonne. La valeur de cette propriété doit être comprise entre 0 et 500. |
| [GetFirstSliceAngle](./getfirstsliceangle/) | Obtient ou définit l'angle de la première tranche de pie-chart ou de doughnut-chart, en degrés (dans le sens des aiguilles d'une montre depuis le vertical). S'applique uniquement aux pie charts, aux 3-D pie charts et aux doughnut charts, avec des valeurs de 0 à 360. |
| [SetFirstSliceAngle](./setfirstsliceangle/) | Obtient ou définit l'angle de la première tranche de pie-chart ou de doughnut-chart, en degrés (dans le sens des aiguilles d'une montre depuis le vertical). S'applique uniquement aux pie charts, aux 3-D pie charts et aux doughnut charts, avec des valeurs de 0 à 360. |
| [GetOverlap](./getoverlap/) | Spécifie comment les barres et les colonnes sont positionnées. Peut être une valeur comprise entre -100 et 100. S'applique uniquement aux 2-D bar charts et aux 2-D column charts. |
| [SetOverlap](./setoverlap/) | Spécifie comment les barres et les colonnes sont positionnées. Peut être une valeur comprise entre -100 et 100. S'applique uniquement aux 2-D bar charts et aux 2-D column charts. |
| [GetSecondPlotSize](./getsecondplotsize/) | Renvoie ou définit la taille de la section secondaire d'un pie of pie chart ou d'un bar of pie chart, en pourcentage de la taille du pie principal. Peut être une valeur de 5 à 200. |
| [SetSecondPlotSize](./setsecondplotsize/) | Renvoie ou définit la taille de la section secondaire d'un pie of pie chart ou d'un bar of pie chart, en pourcentage de la taille du pie principal. Peut être une valeur de 5 à 200. |
| [GetSplitType](./getsplittype/) | Renvoie ou définit une valeur qui détermine quels points de données se trouvent dans le second pie ou la seconde barre d'un pie of pie ou d'un bar of pie chart. |
| [SetSplitType](./setsplittype/) | Renvoie ou définit une valeur qui détermine quels points de données se trouvent dans le second pie ou la seconde barre d'un pie of pie ou d'un bar of pie chart. |
| [GetSplitValue](./getsplitvalue/) | Renvoie ou définit une valeur qui doit être utilisée pour déterminer quels points de données se trouvent dans le second pie ou la seconde barre d'un pie of pie ou d'un bar of pie chart. |
| [SetSplitValue](./setsplitvalue/) | Renvoie ou définit une valeur qui doit être utilisée pour déterminer quels points de données se trouvent dans le second pie ou la seconde barre d'un pie of pie ou d'un bar of pie chart. |
| [IsAutoSplit](./isautosplit/) | Indique si la valeur seuil est automatique. |
| [GetBubbleScale](./getbubblescale/) | Obtient ou définit le facteur d'échelle pour les bulles dans le groupe de graphiques spécifié. Il peut s'agir d'une valeur entière de 0 (zéro) à 300, correspondant à un pourcentage de la taille par défaut. S'applique uniquement aux bubble charts. |
| [SetBubbleScale](./setbubblescale/) | Obtient ou définit le facteur d'échelle pour les bulles dans le groupe de graphiques spécifié. Il peut s'agir d'une valeur entière de 0 (zéro) à 300, correspondant à un pourcentage de la taille par défaut. S'applique uniquement aux bubble charts. |
| [GetSizeRepresents](./getsizerepresents/) | Obtient ou définit ce que représente la taille de la bulle sur un bubble chart. |
| [SetSizeRepresents](./setsizerepresents/) | Obtient ou définit ce que représente la taille de la bulle sur un bubble chart. |
| [GetShowNegativeBubbles](./getshownegativebubbles/) | Vrai si des bulles négatives sont affichées pour le groupe de graphiques. Valide uniquement pour les bubble charts. |
| [SetShowNegativeBubbles](./setshownegativebubbles/) | Vrai si des bulles négatives sont affichées pour le groupe de graphiques. Valide uniquement pour les bubble charts. |
| [GetDoughnutHoleSize](./getdoughnutholesize/) | Renvoie ou définit la taille du trou dans un groupe de doughnut chart. La taille du trou est exprimée en pourcentage de la taille du graphique, entre 10 et 90 pour cent. |
| [SetDoughnutHoleSize](./setdoughnutholesize/) | Renvoie ou définit la taille du trou dans un groupe de doughnut chart. La taille du trou est exprimée en pourcentage de la taille du graphique, entre 10 et 90 pour cent. |
| [GetExplosion](./getexplosion/) | La distance d'une tranche de pie ouverte du centre du pie chart est exprimée en pourcentage du diamètre du pie. |
| [SetExplosion](./setexplosion/) | La distance d'une tranche de pie ouverte du centre du pie chart est exprimée en pourcentage du diamètre du pie. |
| [GetHasRadarAxisLabels](./gethasradaraxislabels/) | Vrai si un radar chart possède des étiquettes d'axe de catégorie. S'applique uniquement aux radar charts. |
| [SetHasRadarAxisLabels](./sethasradaraxislabels/) | Vrai si un radar chart possède des étiquettes d'axe de catégorie. S'applique uniquement aux radar charts. |
| [GetHasLeaderLines](./gethasleaderlines/) | Vrai si la série possède des leader lines. |
| [SetHasLeaderLines](./sethasleaderlines/) | Vrai si la série possède des leader lines. |
| [GetLeaderLines](./getleaderlines/) | Représente les leader lines sur un chart. Les leader lines relient les étiquettes de données aux points de données. Cet objet n'est pas une collection ; il n'existe aucun objet qui représente une seule leader line. |
| [GetLegendEntry](./getlegendentry/) | Obtient l'entrée de légende correspondant à cette série. |
| [GetShapeProperties](./getshapeproperties/) | Obtient l'objet ShapePropertyCollection qui contient les propriétés de forme visuelles de la Series. |
