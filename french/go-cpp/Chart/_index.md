---
title: "Chart Classe"
linktitle: "Chart"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Chart classe. Encapsule l'objet qui représente le chart en Go."
type: docs
weight: 200
url: /fr/go-cpp/chart/
---

## Chart class

Encapsule l'objet qui représente un graphique Excel unique.

```go

type Chart struct  {
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
| [GetStyle](./getstyle/) | Obtient et définit le style intégré. |
| [SetStyle](./setstyle/) | Obtient et définit le style intégré. |
| [GetChartObject](./getchartobject/) | Représente le chartShape ; |
| [GetHidePivotFieldButtons](./gethidepivotfieldbuttons/) | Indique s'il faut masquer les boutons de champ du tableau croisé dynamique uniquement lorsque le graphique est PivotChart. |
| [SetHidePivotFieldButtons](./sethidepivotfieldbuttons/) | Indique s'il faut masquer les boutons de champ du tableau croisé dynamique uniquement lorsque le graphique est PivotChart. |
| [GetPivotOptions](./getpivotoptions/) | Spécifie les contrôles de pivot qui apparaissent sur le graphique |
| [GetPivotSource](./getpivotsource/) | La source est les données du tableau croisé dynamique. Si PivotSource n'est pas vide, le graphique est PivotChart. |
| [SetPivotSource](./setpivotsource/) | La source est les données du tableau croisé dynamique. Si PivotSource n'est pas vide, le graphique est PivotChart. |
| [IsCellReferedByChart](./iscellreferedbychart/) | Renvoie si la cellule référencée par le graphique. |
| [IsChartDataChanged](./ischartdatachanged/) | Détecte si la source de données d'un graphique a changé. |
| [GetPlotBy](./getplotby/) | Obtient et définit si le tracé se fait par ligne ou par colonne. |
| [RefreshPivotData](./refreshpivotdata/) | Actualise les données du graphique à partir du tableau croisé dynamique. |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | Obtient et définit comment tracer les cellules vides. |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | Obtient et définit comment tracer les cellules vides. |
| [GetPlotVisibleCellsOnly](./getplotvisiblecellsonly/) | Indique s'il faut tracer uniquement les cellules visibles. |
| [SetPlotVisibleCellsOnly](./setplotvisiblecellsonly/) | Indique s'il faut tracer uniquement les cellules visibles. |
| [GetDisplayNaAsBlank](./getdisplaynaasblank/) | Indique s'il faut afficher #N/A comme une valeur vide. |
| [SetDisplayNaAsBlank](./setdisplaynaasblank/) | Indique s'il faut afficher #N/A comme une valeur vide. |
| [GetName](./getname/) | Obtient et définit le nom du graphique. |
| [SetName](./setname/) | Obtient et définit le nom du graphique. |
| [GetSizeWithWindow](./getsizewithwindow/) | Vrai si Microsoft Excel redimensionne le graphique pour correspondre à la taille de la fenêtre de la feuille de graphique. |
| [SetSizeWithWindow](./setsizewithwindow/) | Vrai si Microsoft Excel redimensionne le graphique pour correspondre à la taille de la fenêtre de la feuille de graphique. |
| [GetWorksheet](./getworksheet/) | Obtient la feuille de calcul qui contient ce graphique. |
| [GetShapes](./getshapes/) | Renvoie toutes les formes de dessin dans ce graphique. |
| [GetPrintSize](./getprintsize/) | Obtient et définit la taille du graphique imprimé. |
| [SetPrintSize](./setprintsize/) | Obtient et définit la taille du graphique imprimé. |
| [ChangeTemplate](./changetemplate/) | Modifiez le type de graphique avec un modèle prédéfini. |
| [GetType](./gettype/) | Obtient ou définit le type d'un graphique. |
| [SetType](./settype/) | Obtient ou définit le type d'un graphique. |
| [Move](./move/) | Déplace le graphique vers un emplacement spécifié. |
| [GetNSeries](./getnseries/) | Obtient une collection SeriesCollection représentant les séries de données dans le graphique. |
| [GetFilteredNSeries](./getfilterednseries/) | Obtient une collection SeriesCollection représentant les séries de données filtrées dans le graphique. |
| [GetTitle](./gettitle/) | Obtient le titre du graphique. |
| [GetSubTitle](./getsubtitle/) | Obtient le sous-titre du graphique. S'applique uniquement aux fichiers ODS. |
| [GetPlotArea](./getplotarea/) | Obtient la zone de tracé du graphique qui comprend les libellés des graduations des axes. |
| [GetChartArea](./getchartarea/) | Obtient la zone du graphique dans la feuille de calcul. |
| [GetCategoryAxis](./getcategoryaxis/) | Obtient l'axe X du graphique. |
| [GetValueAxis](./getvalueaxis/) | Obtient l'axe Y du graphique. |
| [GetSecondValueAxis](./getsecondvalueaxis/) | Obtient le deuxième axe Y du graphique. |
| [GetSecondCategoryAxis](./getsecondcategoryaxis/) | Obtient le deuxième axe X du graphique. |
| [GetSeriesAxis](./getseriesaxis/) | Obtient l'axe des séries du graphique. |
| [GetLegend](./getlegend/) | Obtient la légende du graphique. |
| [GetChartDataTable](./getchartdatatable/) | Représente le tableau de données du graphique. |
| [GetShowLegend](./getshowlegend/) | Obtient ou définit une valeur indiquant si la légende du graphique doit être affichée. La valeur par défaut est vraie. |
| [SetShowLegend](./setshowlegend/) | Obtient ou définit une valeur indiquant si la légende du graphique doit être affichée. La valeur par défaut est vraie. |
| [IsRectangularCornered](./isrectangularcornered/) | Obtient ou définit une valeur indiquant si la zone du graphique a des coins rectangulaires. La valeur par défaut est vraie. |
| [SetIsRectangularCornered](./setisrectangularcornered/) | Obtient ou définit une valeur indiquant si la zone du graphique a des coins rectangulaires. La valeur par défaut est vraie. |
| [GetShowDataTable](./getshowdatatable/) | Obtient ou définit une valeur indiquant si le graphique affiche un tableau de données. |
| [SetShowDataTable](./setshowdatatable/) | Obtient ou définit une valeur indiquant si le graphique affiche un tableau de données. |
| [GetFirstSliceAngle](./getfirstsliceangle/) | Obtient ou définit l'angle de la première tranche de graphique circulaire ou de beignet, en degrés (dans le sens des aiguilles d'une montre depuis la verticale). S'applique uniquement aux graphiques circulaires, 3D circulaires et de beignet, de 0 à 360. |
| [SetFirstSliceAngle](./setfirstsliceangle/) | Obtient ou définit l'angle de la première tranche de graphique circulaire ou de beignet, en degrés (dans le sens des aiguilles d'une montre depuis la verticale). S'applique uniquement aux graphiques circulaires, 3D circulaires et de beignet, de 0 à 360. |
| [GetGapWidth](./getgapwidth/) | Renvoie ou définit l'espace entre les groupes de barres ou de colonnes, en pourcentage de la largeur de la barre ou de la colonne. La valeur de cette propriété doit être comprise entre 0 et 500. |
| [SetGapWidth](./setgapwidth/) | Renvoie ou définit l'espace entre les groupes de barres ou de colonnes, en pourcentage de la largeur de la barre ou de la colonne. La valeur de cette propriété doit être comprise entre 0 et 500. |
| [GetGapDepth](./getgapdepth/) | Obtient ou définit la distance entre les séries de données dans un graphique 3D, en pourcentage de la largeur du marqueur. La valeur de cette propriété doit être comprise entre 0 et 500. |
| [SetGapDepth](./setgapdepth/) | Obtient ou définit la distance entre les séries de données dans un graphique 3D, en pourcentage de la largeur du marqueur. La valeur de cette propriété doit être comprise entre 0 et 500. |
| [Calculate](./calculate/) | Calcule les positions personnalisées de la zone de tracé et des axes si leurs positions sont attribuées automatiquement. |
| [Calculate_ChartCalculateOptions](./calculate_chartcalculateoptions/) | Calcule la position personnalisée de la zone de tracé, des axes si leur position est attribuée automatiquement, avec les options de calcul du graphique. |
| [GetFloor](./getfloor/) | Renvoie un objet Floor qui représente les parois d'un graphique 3D. |
| [GetWalls](./getwalls/) | Renvoie un objet Walls qui représente les parois d'un graphique 3D. |
| [GetBackWall](./getbackwall/) | Renvoie un objet Walls qui représente la paroi arrière d'un graphique 3D. |
| [GetSideWall](./getsidewall/) | Renvoie un objet Walls qui représente la paroi latérale d'un graphique 3D. |
| [GetWallsAndGridlines2D](./getwallsandgridlines2d/) | Vrai si les lignes de grille sont dessinées en deux dimensions sur un graphique 3D. |
| [SetWallsAndGridlines2D](./setwallsandgridlines2d/) | Vrai si les lignes de grille sont dessinées en deux dimensions sur un graphique 3D. |
| [GetRotationAngle](./getrotationangle/) | Représente la rotation de la vue du graphique 3D (la rotation de la zone de tracé autour de l'axe z, en degrés). |
| [SetRotationAngle](./setrotationangle/) | Représente la rotation de la vue du graphique 3D (la rotation de la zone de tracé autour de l'axe z, en degrés). |
| [GetElevation](./getelevation/) | Représente l'élévation de la vue du graphique 3D, en degrés. |
| [SetElevation](./setelevation/) | Représente l'élévation de la vue du graphique 3D, en degrés. |
| [GetRightAngleAxes](./getrightangleaxes/) | Vrai si les axes du graphique sont perpendiculaires. S'applique uniquement aux graphiques 3D (sauf Column3D et les graphiques circulaires 3D). |
| [SetRightAngleAxes](./setrightangleaxes/) | Vrai si les axes du graphique sont perpendiculaires. S'applique uniquement aux graphiques 3D (sauf Column3D et les graphiques circulaires 3D). |
| [GetAutoScaling](./getautoscaling/) | Vrai si Microsoft Excel met à l'échelle un graphique 3D afin qu'il soit plus proche en taille du graphique 2D équivalent. La propriété RightAngleAxes doit être vraie. |
| [SetAutoScaling](./setautoscaling/) | Vrai si Microsoft Excel met à l'échelle un graphique 3D afin qu'il soit plus proche en taille du graphique 2D équivalent. La propriété RightAngleAxes doit être vraie. |
| [GetHeightPercent](./getheightpercent/) | Renvoie ou définit la hauteur d'un graphique 3D en pourcentage de la largeur du graphique (entre 5 et 500 %). |
| [SetHeightPercent](./setheightpercent/) | Renvoie ou définit la hauteur d'un graphique 3D en pourcentage de la largeur du graphique (entre 5 et 500 %). |
| [GetPerspective](./getperspective/) | Renvoie ou définit la perspective de la vue du graphique tridimensionnel. Doit être comprise entre 0 et 100. Cette propriété est ignorée si la propriété RightAngleAxes est vraie. |
| [SetPerspective](./setperspective/) | Renvoie ou définit la perspective de la vue du graphique tridimensionnel. Doit être comprise entre 0 et 100. Cette propriété est ignorée si la propriété RightAngleAxes est vraie. |
| [GetIs3D](./getis3d/) | Indique si le graphique est un graphique 3D. |
| [GetDepthPercent](./getdepthpercent/) | Représente la profondeur d'un graphique 3D en pourcentage de la largeur du graphique (entre 20 et 2000 %). |
| [SetDepthPercent](./setdepthpercent/) | Représente la profondeur d'un graphique 3D en pourcentage de la largeur du graphique (entre 20 et 2000 %). |
| [ToImage_String](./toimage_string/) | Crée l'image du graphique et l'enregistre dans un fichier. L'extension du nom de fichier détermine le format de l'image. |
| [ToImage_String_ImageType](./toimage_string_imagetype/) | Crée l'image du graphique et l'enregistre dans un fichier du type d'image spécifié. |
| [ToImage_Int64](./toimage_int64/) | Crée l'image du graphique et l'enregistre dans un flux au format Jpeg. |
| [ToImage_ImageType](./toimage_imagetype/) | Crée l'image du graphique et l'enregistre dans un flux au format spécifié. |
| [ToPdf_String](./topdf_string/) | Enregistre le graphique dans un fichier PDF. |
| [ToPdf_String_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_string_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | Enregistre le graphique dans un fichier PDF. |
| [ToPdf](./topdf/) | Crée le PDF du graphique et l'enregistre dans un flux. |
| [ToPdf_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | Crée le PDF du graphique et l'enregistre dans un flux. |
| [ToImage_String_ImageOrPrintOptions](./toimage_string_imageorprintoptions/) | Crée l'image du graphique et l'enregistre dans un fichier. L'extension du nom de fichier détermine le format de l'image. |
| [ToImage_ImageOrPrintOptions](./toimage_imageorprintoptions/) | Crée l'image du graphique et l'enregistre dans un flux au format spécifié. |
| [GetActualSize](./getactualsize/) | Obtient la taille réelle du graphique en pixels. |
| [GetPlacement](./getplacement/) | Représente la façon dont le graphique est attaché aux cellules en dessous. |
| [SetPlacement](./setplacement/) | Représente la façon dont le graphique est attaché aux cellules en dessous. |
| [GetPageSetup](./getpagesetup/) | Représente la description de la mise en page dans ce graphique. |
| [HasAxis](./hasaxis/) | Renvoie quels axes existent sur le graphique. |
| [SwitchRowColumn](./switchrowcolumn/) | Bascule les lignes/colonnes. |
| [GetChartDataRange](./getchartdatarange/) | Obtient la plage de source de données du graphique. |
| [SetChartDataRange](./setchartdatarange/) | Spécifie la plage de données pour un graphique. |
| [GetLine](./getline/) | Obtient la ligne. |
