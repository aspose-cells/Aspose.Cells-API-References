---
title: "Classe SparklineGroup"
linktitle: "SparklineGroup"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe SparklineGroup. Encapsule l'objet qui représente sparklinegroup en Go."
type: docs
weight: 200
url: /fr/go-cpp/sparklinegroup/
---

## SparklineGroup class

<see cref=\"Sparkline\"/> est organisé en un groupe de sparkline.Un SparklineGroup contient un nombre variable d'éléments sparkline.Un groupe de sparkline spécifie le type, les paramètres d'affichage et les paramètres d'axe pour les sparklines.

```go

type SparklineGroup struct  {
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
| [ResetRanges](./resetranges/) | Réinitialise la plage de données et la plage d'emplacement du groupe de sparkline.Cette méthode effacera les éléments sparkline originaux du groupe et créera de nouveaux éléments sparkline pour les nouvelles plages. |
| [GetPresetStyle](./getpresetstyle/) | Obtient et définit le type de style prédéfini du groupe de sparkline. |
| [SetPresetStyle](./setpresetstyle/) | Obtient et définit le type de style prédéfini du groupe de sparkline. |
| [GetSparklines](./getsparklines/) | Obtient la collection d'objets Sparkline. |
| [GetType](./gettype/) | Indique le type de sparkline du groupe de sparkline. |
| [SetType](./settype/) | Indique le type de sparkline du groupe de sparkline. |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | Indique comment tracer les cellules vides. |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | Indique comment tracer les cellules vides. |
| [GetDisplayHidden](./getdisplayhidden/) | Indique s'il faut afficher les données dans les lignes et colonnes masquées. |
| [SetDisplayHidden](./setdisplayhidden/) | Indique s'il faut afficher les données dans les lignes et colonnes masquées. |
| [GetShowHighPoint](./getshowhighpoint/) | Indique s'il faut mettre en évidence les points les plus élevés des données dans le groupe de sparkline. |
| [SetShowHighPoint](./setshowhighpoint/) | Indique s'il faut mettre en évidence les points les plus élevés des données dans le groupe de sparkline. |
| [GetHighPointColor](./gethighpointcolor/) | Obtient et définit la couleur des points les plus élevés des données dans le groupe de sparkline. |
| [SetHighPointColor](./sethighpointcolor/) | Obtient et définit la couleur des points les plus élevés des données dans le groupe de sparkline. |
| [GetShowLowPoint](./getshowlowpoint/) | Indique s'il faut mettre en évidence les points les plus bas des données dans le groupe de sparkline. |
| [SetShowLowPoint](./setshowlowpoint/) | Indique s'il faut mettre en évidence les points les plus bas des données dans le groupe de sparkline. |
| [GetLowPointColor](./getlowpointcolor/) | Obtient et définit la couleur des points les plus bas des données dans le groupe de sparkline. |
| [SetLowPointColor](./setlowpointcolor/) | Obtient et définit la couleur des points les plus bas des données dans le groupe de sparkline. |
| [GetShowNegativePoints](./getshownegativepoints/) | Indique s'il faut mettre en évidence les valeurs négatives du groupe de sparkline avec une couleur ou un marqueur différent. |
| [SetShowNegativePoints](./setshownegativepoints/) | Indique s'il faut mettre en évidence les valeurs négatives du groupe de sparkline avec une couleur ou un marqueur différent. |
| [GetNegativePointsColor](./getnegativepointscolor/) | Obtient et définit la couleur des valeurs négatives du groupe de sparkline. |
| [SetNegativePointsColor](./setnegativepointscolor/) | Obtient et définit la couleur des valeurs négatives du groupe de sparkline. |
| [GetShowFirstPoint](./getshowfirstpoint/) | Indique s'il faut mettre en évidence le premier point de données dans le groupe de sparkline. |
| [SetShowFirstPoint](./setshowfirstpoint/) | Indique s'il faut mettre en évidence le premier point de données dans le groupe de sparkline. |
| [GetFirstPointColor](./getfirstpointcolor/) | Obtient et définit la couleur du premier point de données dans le groupe de sparkline. |
| [SetFirstPointColor](./setfirstpointcolor/) | Obtient et définit la couleur du premier point de données dans le groupe de sparkline. |
| [GetShowLastPoint](./getshowlastpoint/) | Indique s'il faut mettre en évidence le dernier point de données dans le groupe de sparkline. |
| [SetShowLastPoint](./setshowlastpoint/) | Indique s'il faut mettre en évidence le dernier point de données dans le groupe de sparkline. |
| [GetLastPointColor](./getlastpointcolor/) | Obtient et définit la couleur du dernier point de données dans le groupe de sparkline. |
| [SetLastPointColor](./setlastpointcolor/) | Obtient et définit la couleur du dernier point de données dans le groupe de sparkline. |
| [GetShowMarkers](./getshowmarkers/) | Indique s'il faut mettre en évidence chaque point dans chaque sparkline linéaire du groupe de sparkline. |
| [SetShowMarkers](./setshowmarkers/) | Indique s'il faut mettre en évidence chaque point dans chaque sparkline linéaire du groupe de sparkline. |
| [GetMarkersColor](./getmarkerscolor/) | Obtient et définit la couleur des points dans chaque sparkline linéaire du groupe de sparkline. |
| [SetMarkersColor](./setmarkerscolor/) | Obtient et définit la couleur des points dans chaque sparkline linéaire du groupe de sparkline. |
| [GetSeriesColor](./getseriescolor/) | Obtient et définit la couleur des sparklines du groupe de sparkline. |
| [SetSeriesColor](./setseriescolor/) | Obtient et définit la couleur des sparklines du groupe de sparkline. |
| [GetPlotRightToLeft](./getplotrighttoleft/) | Indique si les données du tracé sont de droite à gauche. |
| [SetPlotRightToLeft](./setplotrighttoleft/) | Indique si les données du tracé sont de droite à gauche. |
| [GetLineWeight](./getlineweight/) | Obtient et définit l'épaisseur de ligne dans chaque sparkline linéaire du groupe de sparkline, en unité de points. |
| [SetLineWeight](./setlineweight/) | Obtient et définit l'épaisseur de ligne dans chaque sparkline linéaire du groupe de sparkline, en unité de points. |
| [GetHorizontalAxisColor](./gethorizontalaxiscolor/) | Obtient et définit la couleur de l'axe horizontal du groupe de sparkline. |
| [SetHorizontalAxisColor](./sethorizontalaxiscolor/) | Obtient et définit la couleur de l'axe horizontal du groupe de sparkline. |
| [GetShowHorizontalAxis](./getshowhorizontalaxis/) | Indique s'il faut afficher l'axe horizontal du sparkline.L'axe horizontal apparaît si le sparkline possède des données qui traversent l'axe zéro. |
| [SetShowHorizontalAxis](./setshowhorizontalaxis/) | Indique s'il faut afficher l'axe horizontal du sparkline.L'axe horizontal apparaît si le sparkline possède des données qui traversent l'axe zéro. |
| [GetHorizontalAxisDateRange](./gethorizontalaxisdaterange/) | Représente la plage qui contient les valeurs de date pour les données du sparkline. |
| [SetHorizontalAxisDateRange](./sethorizontalaxisdaterange/) | Représente la plage qui contient les valeurs de date pour les données du sparkline. |
| [GetVerticalAxisMaxValueType](./getverticalaxismaxvaluetype/) | Représente le type de valeur maximale de l'axe vertical. |
| [SetVerticalAxisMaxValueType](./setverticalaxismaxvaluetype/) | Représente le type de valeur maximale de l'axe vertical. |
| [GetVerticalAxisMaxValue](./getverticalaxismaxvalue/) | Obtient et définit la valeur maximale personnalisée pour l'axe vertical. |
| [SetVerticalAxisMaxValue_Double](./setverticalaxismaxvalue_double/) | Obtient et définit la valeur maximale personnalisée pour l'axe vertical. |
| [SetVerticalAxisMaxValue_SparklineAxisMinMaxType_Double](./setverticalaxismaxvalue_sparklineaxisminmaxtype_double/) | Définit la valeur maximale personnalisée pour l'axe vertical du sparkline avec le type de valeur d'axe spécifié. |
| [SetVerticalAxisMinValue_SparklineAxisMinMaxType_Double](./setverticalaxisminvalue_sparklineaxisminmaxtype_double/) | Définit la valeur minimale personnalisée pour l'axe vertical du sparkline avec le type de valeur d'axe spécifié. |
| [GetVerticalAxisMinValueType](./getverticalaxisminvaluetype/) | Représente le type de valeur minimale de l'axe vertical. |
| [SetVerticalAxisMinValueType](./setverticalaxisminvaluetype/) | Représente le type de valeur minimale de l'axe vertical. |
| [GetVerticalAxisMinValue](./getverticalaxisminvalue/) | Obtient et définit la valeur minimale personnalisée pour l'axe vertical. |
| [SetVerticalAxisMinValue_Double](./setverticalaxisminvalue_double/) | Obtient et définit la valeur minimale personnalisée pour l'axe vertical. |
