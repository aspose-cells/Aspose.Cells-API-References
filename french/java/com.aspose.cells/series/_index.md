---
title: "Series"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente une série de données unique dans un graphique."
type: docs
url: /fr/java/com.aspose.cells/series/
---

**Inheritance:**
java.lang.Object
```
public class Series
```

Encapsule l'objet qui représente une série de données unique dans un graphique.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         int seriesIndex = chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         Series series = chart.getNSeries().get(seriesIndex);
         //Setting the values of the series.
         series.setValues("=B1:B4");
         //Changing the chart type of the series.
         series.setType(ChartType.LINE);
         //Setting marker properties.
         series.getMarker().setMarkerStyle(ChartMarkerType.CIRCLE);
         series.getMarker().setForegroundColorSetType(FormattingType.AUTOMATIC);
         series.getMarker().setForegroundColor(com.aspose.cells.Color.getBlack());
         series.getMarker().setBackgroundColorSetType(FormattingType.AUTOMATIC);
 
         //do your business
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Représente la zone d'arrière-plan de l'objet Series. |
| [getBar3DShapeType()](#getBar3DShapeType--) | Obtient le type de forme 3D utilisé avec le graphique à barres ou à colonnes 3D. |
| [getBorder()](#getBorder--) | Représente la bordure d'un objet Series. |
| [getBubbleScale()](#getBubbleScale--) | Obtient le facteur d'échelle des bulles dans le groupe de graphiques spécifié. |
| [getBubbleSizeRepresents()](#getBubbleSizeRepresents--) | Obtient ce que représente la taille des bulles sur un graphique à bulles. |
| [getBubbleSizes()](#getBubbleSizes--) | Obtient les valeurs de taille des bulles de la série de graphique. |
| [getCachedCategoryValues()](#getCachedCategoryValues--) | Obtient les valeurs de catégorie mises en cache pour la série |
| [getCachedValues()](#getCachedValues--) | Obtient les valeurs mises en cache pour la série |
| [getCategoryValues()](#getCategoryValues--) | Obtient les valeurs de catégorie réelles utilisées pour tracer chaque point de cette série dans le graphique. |
| [getClass()](#getClass--) |  |
| [getCountOfDataValues()](#getCountOfDataValues--) | Obtient le nombre de valeurs de données. |
| [getDataLabels()](#getDataLabels--) | Représente l'objet DataLabels pour l'ASeries spécifié. |
| [getDisplayName()](#getDisplayName--) | Obtient le nom de la série affiché sur le graphique. |
| [getDoughnutHoleSize()](#getDoughnutHoleSize--) | Renvoie ou définit la taille du trou dans un groupe de graphique en anneau. |
| [getDownBars()](#getDownBars--) | Renvoie un objet [DropBars](../../com.aspose.cells/dropbars) qui représente les barres descendantes sur un graphique en ligne. |
| [getDropLines()](#getDropLines--) | Renvoie un objet [Line](../../com.aspose.cells/line) qui représente les lignes de chute pour une série sur le graphique en ligne ou le graphique en aires. |
| [getExplosion()](#getExplosion--) | La distance d'une tranche de diagramme circulaire ouverte du centre du diagramme circulaire est exprimée en pourcentage du diamètre du diagramme. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | Obtient l'angle de la première tranche de diagramme circulaire ou de diagramme en anneau, en degrés (dans le sens des aiguilles d'une montre à partir du vertical). |
| [getGapWidth()](#getGapWidth--) | Renvoie ou définit l'espace entre les groupes de barres ou de colonnes, en pourcentage de la largeur de la barre ou de la colonne. |
| [getHas3DEffect()](#getHas3DEffect--) | Vrai si la série a une apparence tridimensionnelle. |
| [getHiLoLines()](#getHiLoLines--) | Renvoie un objet HiLoLines qui représente les lignes haut-bas pour une série sur un graphique en ligne. |
| [getLayoutProperties()](#getLayoutProperties--) | Représente les propriétés de la mise en page. |
| [getLeaderLines()](#getLeaderLines--) | Représente les lignes directrices sur un graphique. |
| [getLegendEntry()](#getLegendEntry--) | Obtient l'entrée de légende correspondant à cette série. |
| [getMarker()](#getMarker--) | Obtient le [getMarker()](../../com.aspose.cells/series\#getMarker--). |
| [getName()](#getName--) | Obtient le nom de la série de données. |
| [getOverlap()](#getOverlap--) | Spécifie comment les barres et les colonnes sont positionnées. |
| [getPlotOnSecondAxis()](#getPlotOnSecondAxis--) | Indique si cette série est tracée sur le deuxième axe des valeurs. |
| [getPointValues()](#getPointValues--) | Obtient les valeurs réelles utilisées pour tracer chaque point de cette série dans le graphique. |
| [getPoints()](#getPoints--) | Obtient la collection de points d’une série dans un graphique. |
| [getSecondPlotSize()](#getSecondPlotSize--) | Renvoie ou définit la taille de la section secondaire d’un diagramme « pie of pie » ou d’un diagramme « bar of pie », en pourcentage de la taille du diagramme principal. |
| [getSeriesLines()](#getSeriesLines--) | Renvoie un objet SeriesLines qui représente les lignes de série pour un diagramme à barres empilées ou un diagramme à colonnes empilées. |
| [getShadow()](#getShadow--) | Vrai si la série possède une ombre. |
| [getShapeProperties()](#getShapeProperties--) | Obtient l’objet [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) qui contient les propriétés visuelles de forme de la série. |
| [getShowNegativeBubbles()](#getShowNegativeBubbles--) | Vrai si les bulles négatives sont affichées pour le groupe de graphique. |
| [getSizeRepresents()](#getSizeRepresents--) | Obtient ce que représente la taille des bulles sur un graphique à bulles. |
| [getSmooth()](#getSmooth--) | Représente le lissage de courbe. |
| [getSplitType()](#getSplitType--) | Renvoie ou définit une valeur qui indique comment déterminer quels points de données se trouvent dans le deuxième secteur ou la deuxième barre d’un diagramme « pie of pie » ou « bar of pie ». |
| [getSplitValue()](#getSplitValue--) | Renvoie ou définit une valeur qui doit être utilisée pour déterminer quels points de données se trouvent dans le deuxième secteur ou la deuxième barre d’un diagramme « pie of pie » ou « bar of pie ». |
| [getTrendLines()](#getTrendLines--) | Renvoie toutes les lignes de tendance de cette série. |
| [getType()](#getType--) | Obtient le type d’une série de données. |
| [getUpBars()](#getUpBars--) | Renvoie un objet DropBars qui représente les barres ascendantes sur un diagramme en ligne. |
| [getValues()](#getValues--) | Représente les valeurs Y de cette série de graphique. |
| [getValuesFormatCode()](#getValuesFormatCode--) | Représente le code de format de la liste de nombres des valeurs. |
| [getXErrorBar()](#getXErrorBar--) | Représente la barre d’erreur en direction X de la série. |
| [getXValues()](#getXValues--) | Représente les valeurs X de cette série de graphique. |
| [getXValuesFormatCode()](#getXValuesFormatCode--) | Représente le code de format de la liste de nombres des valeurs X. |
| [getYErrorBar()](#getYErrorBar--) | Représente la barre d’erreur en direction Y de la série. |
| [hasDropLines()](#hasDropLines--) | Vrai si le graphique possède des lignes de chute. |
| [hasHiLoLines()](#hasHiLoLines--) | Vrai si le diagramme en ligne possède des lignes haut-bas. |
| [hasLeaderLines()](#hasLeaderLines--) | Vrai si la série possède des lignes de repère. |
| [hasRadarAxisLabels()](#hasRadarAxisLabels--) | Vrai si un diagramme radar possède des étiquettes d’axe de catégorie. |
| [hasSeriesLines()](#hasSeriesLines--) | Vrai si un graphique à colonnes empilées ou un graphique à barres possède des lignes de séries ou si un graphique Pie of Pie ou Bar of Pie possède des lignes de connexion entre les deux sections. |
| [hasUpDownBars()](#hasUpDownBars--) | Vrai si un graphique en lignes possède des barres hautes et basses. |
| [hashCode()](#hashCode--) |  |
| [isAutoSplit()](#isAutoSplit--) | Indique si la valeur du seuil est automatique. |
| [isColorVaried()](#isColorVaried--) | Indique si la couleur des points varie. |
| [isFiltered()](#isFiltered--) | Indique si la série est sélectionnée ou filtrée. |
| [isVerticalValues()](#isVerticalValues--) | Indique si la source de données est verticale. |
| [move(int count)](#move-int-) | Déplace la série vers le haut ou vers le bas. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBar3DShapeType(int value)](#setBar3DShapeType-int-) | Définit le type de forme 3D utilisé avec le graphique à barres ou à colonnes 3D. |
| [setBubbleScale(int value)](#setBubbleScale-int-) | Définit le facteur d'échelle des bulles dans le groupe de graphiques spécifié. |
| [setBubbleSizeRepresents(int value)](#setBubbleSizeRepresents-int-) | Obtient ce que représente la taille des bulles sur un graphique à bulles. |
| [setBubbleSizes(String value)](#setBubbleSizes-java.lang.String-) | Définit les valeurs de taille des bulles de la série de graphique. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Indique si la couleur des points varie. |
| [setDoughnutHoleSize(int value)](#setDoughnutHoleSize-int-) | Renvoie ou définit la taille du trou dans un groupe de graphique en anneau. |
| [setExplosion(int value)](#setExplosion-int-) | La distance d'une tranche de diagramme circulaire ouverte du centre du diagramme circulaire est exprimée en pourcentage du diamètre du diagramme. |
| [setFiltered(boolean value)](#setFiltered-boolean-) | Indique si la série est sélectionnée ou filtrée. |
| [setFirstSliceAngle(short value)](#setFirstSliceAngle-short-) | Définit l'angle de la première tranche de diagramme circulaire ou de donut, en degrés (dans le sens des aiguilles d'une montre depuis la verticale). |
| [setGapWidth(short value)](#setGapWidth-short-) | Renvoie ou définit l'espace entre les groupes de barres ou de colonnes, en pourcentage de la largeur de la barre ou de la colonne. |
| [setHas3DEffect(boolean value)](#setHas3DEffect-boolean-) | Vrai si la série a une apparence tridimensionnelle. |
| [setHasDropLines(boolean value)](#setHasDropLines-boolean-) | Vrai si le graphique possède des lignes de chute. |
| [setHasHiLoLines(boolean value)](#setHasHiLoLines-boolean-) | Vrai si le diagramme en ligne possède des lignes haut-bas. |
| [setHasLeaderLines(boolean value)](#setHasLeaderLines-boolean-) | Vrai si la série possède des lignes de repère. |
| [setHasRadarAxisLabels(boolean value)](#setHasRadarAxisLabels-boolean-) | Vrai si un diagramme radar possède des étiquettes d’axe de catégorie. |
| [setHasSeriesLines(boolean value)](#setHasSeriesLines-boolean-) | Vrai si un graphique à colonnes empilées ou un graphique à barres possède des lignes de séries ou si un graphique Pie of Pie ou Bar of Pie possède des lignes de connexion entre les deux sections. |
| [setHasUpDownBars(boolean value)](#setHasUpDownBars-boolean-) | Vrai si un graphique en lignes possède des barres hautes et basses. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom de la série de données. |
| [setOverlap(short value)](#setOverlap-short-) | Spécifie comment les barres et les colonnes sont positionnées. |
| [setPlotOnSecondAxis(boolean value)](#setPlotOnSecondAxis-boolean-) | Indique si cette série est tracée sur le deuxième axe des valeurs. |
| [setSecondPlotSize(short value)](#setSecondPlotSize-short-) | Renvoie ou définit la taille de la section secondaire d’un diagramme « pie of pie » ou d’un diagramme « bar of pie », en pourcentage de la taille du diagramme principal. |
| [setShadow(boolean value)](#setShadow-boolean-) | Vrai si la série possède une ombre. |
| [setShowNegativeBubbles(boolean value)](#setShowNegativeBubbles-boolean-) | Vrai si les bulles négatives sont affichées pour le groupe de graphique. |
| [setSizeRepresents(int value)](#setSizeRepresents-int-) | Définit ce que représente la taille des bulles sur un graphique à bulles. |
| [setSmooth(boolean value)](#setSmooth-boolean-) | Représente le lissage de courbe. |
| [setSplitType(int value)](#setSplitType-int-) | Renvoie ou définit une valeur qui indique comment déterminer quels points de données se trouvent dans le deuxième secteur ou la deuxième barre d’un diagramme « pie of pie » ou « bar of pie ». |
| [setSplitValue(double value)](#setSplitValue-double-) | Renvoie ou définit une valeur qui doit être utilisée pour déterminer quels points de données se trouvent dans le deuxième secteur ou la deuxième barre d’un diagramme « pie of pie » ou « bar of pie ». |
| [setType(int value)](#setType-int-) | Définit le type d'une série de données. |
| [setValues(String value)](#setValues-java.lang.String-) | Représente les valeurs Y de cette série de graphique. |
| [setValuesFormatCode(String value)](#setValuesFormatCode-java.lang.String-) | Représente le code de format de la liste de nombres des valeurs. |
| [setXValues(String value)](#setXValues-java.lang.String-) | Représente les valeurs X de cette série de graphique. |
| [setXValuesFormatCode(String value)](#setXValuesFormatCode-java.lang.String-) | Représente le code de format de la liste de nombres des valeurs X. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArea() {#getArea--}
```
public Area getArea()
```


Représente la zone d'arrière-plan de l'objet Series.

**Returns:**
[Area](../../com.aspose.cells/area)
### getBar3DShapeType() {#getBar3DShapeType--}
```
public int getBar3DShapeType()
```


Obtient le type de forme 3D utilisé avec le graphique à barres ou à colonnes 3D.

Voir [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Représente la bordure d'un objet Series.

**Returns:**
[Line](../../com.aspose.cells/line)
### getBubbleScale() {#getBubbleScale--}
```
public int getBubbleScale()
```


Obtient le facteur d'échelle des bulles dans le groupe de graphiques spécifié. Il peut s'agir d'une valeur entière de 0 (zéro) à 300, correspondant à un pourcentage de la taille par défaut. S'applique uniquement aux graphiques à bulles.

**Returns:**
int
### getBubbleSizeRepresents() {#getBubbleSizeRepresents--}
```
public int getBubbleSizeRepresents()
```


Obtient ce que représente la taille des bulles sur un graphique à bulles.

Voir [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Aspose.Cells.Charts.Series.SizeRepresents. Cette propriété sera supprimée 12 mois plus tard à compter de JANVIER 2012. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getBubbleSizes() {#getBubbleSizes--}
```
public String getBubbleSizes()
```


Obtient les valeurs de taille des bulles de la série de graphique.

**Remarks**

Uniquement pour [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) ou [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Returns:**
java.lang.String
### getCachedCategoryValues() {#getCachedCategoryValues--}
```
public ArrayList getCachedCategoryValues()
```


Obtient les valeurs de catégorie mises en cache pour la série

**Remarks**

NOTE : Cette propriété est actuellement réservée à un usage interne uniquement. Elle sera modifiée ou supprimée dans la prochaine version.

**Returns:**
java.util.ArrayList
### getCachedValues() {#getCachedValues--}
```
public ArrayList getCachedValues()
```


Obtient les valeurs mises en cache pour la série

**Remarks**

NOTE : Cette propriété est actuellement réservée à un usage interne uniquement. Elle sera modifiée ou supprimée dans la prochaine version.

**Returns:**
java.util.ArrayList
### getCategoryValues() {#getCategoryValues--}
```
public ChartDataValue[][] getCategoryValues()
```


Obtient les valeurs de catégorie réelles utilisées pour tracer chaque point de cette série dans le graphique.

**Remarks**

Cette propriété offre un moyen pratique d'obtenir les valeurs réelles correspondant aux données définies par [getXValues()](../../com.aspose.cells/series\#getXValues--), en particulier lorsque la source de données spécifiée est un lien externe, une formule, ...etc.

**Example**

```
         //Standalone example
         Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Chart chart = worksheet.getCharts().get(0);
         chart.calculate();
         String XValues = chart.getNSeries().get(0).getXValues();
         // XValues may be like "[External.xlsx]Sheet1!$B$2:$C$6" which is complicated
         // for user to get the actual values(the values may be linked to another workbook,
         // or cached in current workbook). Here you can use CategoryValues property
         // to get the category values actually displayed in the Excel interface
         // in the form of a two-dimensional array.
         ChartDataValue[][] v1 = chart.getNSeries().get(0).getCategoryValues();
```

**Returns:**
com.aspose.cells.ChartDataValue[][]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCountOfDataValues() {#getCountOfDataValues--}
```
public int getCountOfDataValues()
```


Obtient le nombre de valeurs de données.

**Returns:**
int
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Représente l'objet DataLabels pour l'ASeries spécifié.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Obtient le nom de la série affiché sur le graphique.

**Returns:**
java.lang.String
### getDoughnutHoleSize() {#getDoughnutHoleSize--}
```
public int getDoughnutHoleSize()
```


Renvoie ou définit la taille du trou dans un groupe de graphique en anneau. La taille du trou est exprimée en pourcentage de la taille du graphique, entre 10 et 90 pour cent.

**Returns:**
int
### getDownBars() {#getDownBars--}
```
public DropBars getDownBars()
```


Renvoie un objet [DropBars](../../com.aspose.cells/dropbars) qui représente les barres descendantes sur un graphique en lignes. S'applique uniquement aux graphiques en lignes.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getDropLines() {#getDropLines--}
```
public Line getDropLines()
```


Renvoie un objet [Line](../../com.aspose.cells/line) qui représente les lignes de repère pour une série sur le graphique en lignes ou le graphique en aires. S'applique uniquement aux graphiques en lignes ou aux graphiques en aires.

**Returns:**
[Line](../../com.aspose.cells/line)
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


La distance d'une tranche de diagramme circulaire ouverte du centre du diagramme circulaire est exprimée en pourcentage du diamètre du diagramme.

**Returns:**
int
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public short getFirstSliceAngle()
```


Obtient l'angle de la première tranche de graphique circulaire ou d'anneau, en degrés (dans le sens des aiguilles d'une montre à partir du vertical). S'applique uniquement aux graphiques circulaires, aux graphiques circulaires 3D et aux graphiques en anneau, avec des valeurs de 0 à 360.

**Returns:**
short
### getGapWidth() {#getGapWidth--}
```
public short getGapWidth()
```


Renvoie ou définit l’espace entre les groupes de barres ou de colonnes, exprimé en pourcentage de la largeur de la barre ou de la colonne. La valeur de cette propriété doit être comprise entre 0 et 500.

**Returns:**
short
### getHas3DEffect() {#getHas3DEffect--}
```
public boolean getHas3DEffect()
```


Vrai si la série a une apparence tridimensionnelle.

**Remarks**

S'applique uniquement aux graphiques [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) ou [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Returns:**
boolean
### getHiLoLines() {#getHiLoLines--}
```
public Line getHiLoLines()
```


Renvoie un objet HiLoLines qui représente les lignes haut-bas pour une série sur un graphique en courbes. S'applique uniquement aux graphiques en courbes.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLayoutProperties() {#getLayoutProperties--}
```
public SeriesLayoutProperties getLayoutProperties()
```


Représente les propriétés de la mise en page.

**Returns:**
[SeriesLayoutProperties](../../com.aspose.cells/serieslayoutproperties)
### getLeaderLines() {#getLeaderLines--}
```
public Line getLeaderLines()
```


Représente les lignes de repère sur un graphique. Les lignes de repère relient les étiquettes de données aux points de données. Cet objet n'est pas une collection ; il n'existe aucun objet qui représente une seule ligne de repère.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


Obtient l'entrée de légende correspondant à cette série.

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


Obtient le [getMarker()](../../com.aspose.cells/series\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getName() {#getName--}
```
public String getName()
```


Obtient le nom de la série de données.

**Example**

```
         //Reference name to a cell
         chart.getNSeries().get(0).setName("=A1");
 
         //Set a string to name
         chart.getNSeries().get(0).setName("First Series");
```

**Returns:**
java.lang.String
### getOverlap() {#getOverlap--}
```
public short getOverlap()
```


Spécifie la façon dont les barres et les colonnes sont positionnées. Peut être une valeur comprise entre -100 et 100. S'applique uniquement aux graphiques à barres 2D et aux graphiques à colonnes 2D.

**Returns:**
short
### getPlotOnSecondAxis() {#getPlotOnSecondAxis--}
```
public boolean getPlotOnSecondAxis()
```


Indique si cette série est tracée sur le deuxième axe des valeurs.

**Returns:**
boolean
### getPointValues() {#getPointValues--}
```
public ChartDataValue[] getPointValues()
```


Obtient les valeurs réelles utilisées pour tracer chaque point de cette série dans le graphique.

**Remarks**

Cette propriété offre un moyen pratique d'obtenir les valeurs réelles correspondant aux données définies par [getValues()](../../com.aspose.cells/series\#getValues--), en particulier lorsque la source de données spécifiée est un lien externe, une formule, etc.

**Example**

```
         Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Chart chart = worksheet.getCharts().get(0);
         chart.calculate();
         String Values = chart.getNSeries().get(0).getValues();
         // Values could be like "[External.xlsx]Sheet1!$A$1:$A$6" which is complicated
         // for user to get the actual values(the values may be linked to another workbook,
         // or cached in current workbook). Here you can use PointValues property
         // to get the values actually displayed in the Excel interface
         // in the form of an array.
         ChartDataValue[] v1 = chart.getNSeries().get(0).getPointValues();
```

**Returns:**
com.aspose.cells.ChartDataValue[]
### getPoints() {#getPoints--}
```
public ChartPointCollection getPoints()
```


Obtient la collection de points d’une série dans un graphique.

**Remarks**

Lorsque le graphique est un diagramme « Pie of Pie » ou « Bar of Pie », le dernier point est le point « other » dans le premier tracé de secteur.

**Returns:**
[ChartPointCollection](../../com.aspose.cells/chartpointcollection)
### getSecondPlotSize() {#getSecondPlotSize--}
```
public short getSecondPlotSize()
```


Renvoie ou définit la taille de la section secondaire d'un graphique « pie of pie » ou « bar of pie », exprimée en pourcentage de la taille du secteur principal. Peut être une valeur comprise entre 5 et 200.

**Returns:**
short
### getSeriesLines() {#getSeriesLines--}
```
public Line getSeriesLines()
```


Renvoie un objet SeriesLines qui représente les lignes de série pour un graphique à barres empilées ou un graphique à colonnes empilées. S'applique uniquement aux graphiques à barres empilées et aux graphiques à colonnes empilées.

**Returns:**
[Line](../../com.aspose.cells/line)
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Vrai si la série possède une ombre.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Obtient l’objet [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) qui contient les propriétés visuelles de forme de la série.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShowNegativeBubbles() {#getShowNegativeBubbles--}
```
public boolean getShowNegativeBubbles()
```


Vrai si les bulles négatives sont affichées pour le groupe de graphiques. Valide uniquement pour les graphiques à bulles.

**Returns:**
boolean
### getSizeRepresents() {#getSizeRepresents--}
```
public int getSizeRepresents()
```


Obtient ce que représente la taille des bulles sur un graphique à bulles.

Voir [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea signifie que la valeur [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) correspond à la surface de la bulle. BubbleSizeRepresents.SizeIsWidth signifie que la valeur [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) correspond à la largeur de la bulle.

**Returns:**
int
### getSmooth() {#getSmooth--}
```
public boolean getSmooth()
```


Représente le lissage de courbe. Vrai si le lissage de courbe est activé pour le graphique en lignes ou le nuage de points. S'applique uniquement aux graphiques en lignes et aux nuages de points avec lignes.

**Returns:**
boolean
### getSplitType() {#getSplitType--}
```
public int getSplitType()
```


Renvoie ou définit une valeur qui indique comment déterminer quels points de données se trouvent dans le deuxième secteur ou la deuxième barre d’un diagramme « pie of pie » ou « bar of pie ».

Voir [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Returns:**
int
### getSplitValue() {#getSplitValue--}
```
public double getSplitValue()
```


Renvoie ou définit une valeur qui doit être utilisée pour déterminer quels points de données se trouvent dans le deuxième secteur ou la deuxième barre d’un diagramme « pie of pie » ou « bar of pie ».

**Returns:**
double
### getTrendLines() {#getTrendLines--}
```
public TrendlineCollection getTrendLines()
```


Renvoie toutes les lignes de tendance de cette série.

**Returns:**
[TrendlineCollection](../../com.aspose.cells/trendlinecollection)
### getType() {#getType--}
```
public int getType()
```


Obtient le type d’une série de données.

Voir [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getUpBars() {#getUpBars--}
```
public DropBars getUpBars()
```


Renvoie un objet DropBars qui représente les barres ascendantes sur un graphique en lignes. S'applique uniquement aux graphiques en lignes.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getValues() {#getValues--}
```
public String getValues()
```


Représente les valeurs Y de cette série de graphique.

**Remarks**

Pour obtenir les valeurs réelles (correspondant à chaque point de cette série) définies par cette propriété, veuillez utiliser [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Returns:**
java.lang.String
### getValuesFormatCode() {#getValuesFormatCode--}
```
public String getValuesFormatCode()
```


Représente le code de format de la liste de nombres des valeurs.

**Returns:**
java.lang.String
### getXErrorBar() {#getXErrorBar--}
```
public ErrorBar getXErrorBar()
```


Représente la barre d’erreur en direction X de la série.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### getXValues() {#getXValues--}
```
public String getXValues()
```


Représente les valeurs X de cette série de graphique.

**Remarks**

Uniquement pour les graphiques en nuage de points et à bulles. Veuillez utiliser [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) pour les autres types de graphiques ; [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) est utilisé pour obtenir les valeurs de catégorie réelles de cette série.

**Returns:**
java.lang.String
### getXValuesFormatCode() {#getXValuesFormatCode--}
```
public String getXValuesFormatCode()
```


Représente le code de format de la liste de nombres des valeurs X.

**Returns:**
java.lang.String
### getYErrorBar() {#getYErrorBar--}
```
public ErrorBar getYErrorBar()
```


Représente la barre d’erreur en direction Y de la série.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### hasDropLines() {#hasDropLines--}
```
public boolean hasDropLines()
```


Vrai si le graphique possède des lignes de chute. S'applique uniquement aux graphiques en lignes ou aux graphiques en aires.

**Returns:**
boolean
### hasHiLoLines() {#hasHiLoLines--}
```
public boolean hasHiLoLines()
```


Vrai si le graphique en lignes possède des lignes haut-bas. S'applique uniquement aux graphiques en lignes.

**Returns:**
boolean
### hasLeaderLines() {#hasLeaderLines--}
```
public boolean hasLeaderLines()
```


Vrai si la série possède des lignes de repère.

**Returns:**
boolean
### hasRadarAxisLabels() {#hasRadarAxisLabels--}
```
public boolean hasRadarAxisLabels()
```


Vrai si un graphique radar possède des étiquettes d'axe de catégorie. S'applique uniquement aux graphiques radar.

**Returns:**
boolean
### hasSeriesLines() {#hasSeriesLines--}
```
public boolean hasSeriesLines()
```


Vrai si un graphique à colonnes empilées ou à barres possède des lignes de série ou si un graphique « Pie of Pie » ou « Bar of Pie » possède des lignes de connexion entre les deux sections. S'applique uniquement aux graphiques à colonnes empilées, aux graphiques à barres, aux graphiques « Pie of Pie » ou « Bar of Pie ».

**Returns:**
boolean
### hasUpDownBars() {#hasUpDownBars--}
```
public boolean hasUpDownBars()
```


Vrai si un graphique en lignes possède des barres haut et bas. S'applique uniquement aux graphiques en lignes.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSplit() {#isAutoSplit--}
```
public boolean isAutoSplit()
```


Indique si la valeur du seuil est automatique.

**Returns:**
boolean
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


Indique si la couleur des points varie. Le graphique doit contenir une seule série ou être un graphique circulaire.

**Returns:**
boolean
### isFiltered() {#isFiltered--}
```
public boolean isFiltered()
```


Indique si la série est sélectionnée ou filtrée. Vrai indique que cette série est filtrée et ne sera pas affichée sur le graphique.

**Returns:**
boolean
### isVerticalValues() {#isVerticalValues--}
```
public boolean isVerticalValues()
```


Indique si la source de données est verticale.

**Returns:**
boolean
### move(int count) {#move-int-}
```
public void move(int count)
```


Déplace la série vers le haut ou vers le bas.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| count | int | Le nombre de déplacements vers le haut ou le bas. Déplacez la série vers le haut si cette valeur est inférieure à zéro ; déplacez-la vers le bas si elle est supérieure à zéro. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBar3DShapeType(int value) {#setBar3DShapeType-int-}
```
public void setBar3DShapeType(int value)
```


Définit le type de forme 3D utilisé avec le graphique à barres ou à colonnes 3D.

Voir [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBubbleScale(int value) {#setBubbleScale-int-}
```
public void setBubbleScale(int value)
```


Définit le facteur d'échelle des bulles dans le groupe de graphiques spécifié. Il peut s'agir d'une valeur entière comprise entre 0 (zéro) et 300, correspondant à un pourcentage de la taille par défaut. S'applique uniquement aux graphiques à bulles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBubbleSizeRepresents(int value) {#setBubbleSizeRepresents-int-}
```
public void setBubbleSizeRepresents(int value)
```


Obtient ce que représente la taille des bulles sur un graphique à bulles.

Voir [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Aspose.Cells.Charts.Series.SizeRepresents. Cette propriété sera supprimée 12 mois plus tard à compter de JANVIER 2012. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBubbleSizes(String value) {#setBubbleSizes-java.lang.String-}
```
public void setBubbleSizes(String value)
```


Définit les valeurs de taille des bulles de la série de graphique.

**Remarks**

Uniquement pour [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) ou [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


Indique si la couleur des points varie. Le graphique doit contenir une seule série ou être un graphique circulaire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDoughnutHoleSize(int value) {#setDoughnutHoleSize-int-}
```
public void setDoughnutHoleSize(int value)
```


Renvoie ou définit la taille du trou dans un groupe de graphique en anneau. La taille du trou est exprimée en pourcentage de la taille du graphique, entre 10 et 90 pour cent.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```


La distance d'une tranche de diagramme circulaire ouverte du centre du diagramme circulaire est exprimée en pourcentage du diamètre du diagramme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setFiltered(boolean value) {#setFiltered-boolean-}
```
public void setFiltered(boolean value)
```


Indique si la série est sélectionnée ou filtrée. Vrai indique que cette série est filtrée et ne sera pas affichée sur le graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFirstSliceAngle(short value) {#setFirstSliceAngle-short-}
```
public void setFirstSliceAngle(short value)
```


Définit l'angle de la première tranche de diagramme circulaire ou de diagramme en anneau, en degrés (dans le sens des aiguilles d'une montre à partir du vertical). S'applique uniquement aux diagrammes circulaires, 3D circulaires et en anneau, avec des valeurs de 0 à 360.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | short |  |

### setGapWidth(short value) {#setGapWidth-short-}
```
public void setGapWidth(short value)
```


Renvoie ou définit l’espace entre les groupes de barres ou de colonnes, exprimé en pourcentage de la largeur de la barre ou de la colonne. La valeur de cette propriété doit être comprise entre 0 et 500.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | short |  |

### setHas3DEffect(boolean value) {#setHas3DEffect-boolean-}
```
public void setHas3DEffect(boolean value)
```


Vrai si la série a une apparence tridimensionnelle.

**Remarks**

S'applique uniquement aux graphiques [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) ou [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasDropLines(boolean value) {#setHasDropLines-boolean-}
```
public void setHasDropLines(boolean value)
```


Vrai si le graphique possède des lignes de chute. S'applique uniquement aux graphiques en lignes ou aux graphiques en aires.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasHiLoLines(boolean value) {#setHasHiLoLines-boolean-}
```
public void setHasHiLoLines(boolean value)
```


Vrai si le graphique en lignes possède des lignes haut-bas. S'applique uniquement aux graphiques en lignes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasLeaderLines(boolean value) {#setHasLeaderLines-boolean-}
```
public void setHasLeaderLines(boolean value)
```


Vrai si la série possède des lignes de repère.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasRadarAxisLabels(boolean value) {#setHasRadarAxisLabels-boolean-}
```
public void setHasRadarAxisLabels(boolean value)
```


Vrai si un graphique radar possède des étiquettes d'axe de catégorie. S'applique uniquement aux graphiques radar.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasSeriesLines(boolean value) {#setHasSeriesLines-boolean-}
```
public void setHasSeriesLines(boolean value)
```


Vrai si un graphique à colonnes empilées ou à barres possède des lignes de série ou si un graphique « Pie of Pie » ou « Bar of Pie » possède des lignes de connexion entre les deux sections. S'applique uniquement aux graphiques à colonnes empilées, aux graphiques à barres, aux graphiques « Pie of Pie » ou « Bar of Pie ».

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasUpDownBars(boolean value) {#setHasUpDownBars-boolean-}
```
public void setHasUpDownBars(boolean value)
```


Vrai si un graphique en lignes possède des barres haut et bas. S'applique uniquement aux graphiques en lignes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Définit le nom de la série de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOverlap(short value) {#setOverlap-short-}
```
public void setOverlap(short value)
```


Spécifie la façon dont les barres et les colonnes sont positionnées. Peut être une valeur comprise entre -100 et 100. S'applique uniquement aux graphiques à barres 2D et aux graphiques à colonnes 2D.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | short |  |

### setPlotOnSecondAxis(boolean value) {#setPlotOnSecondAxis-boolean-}
```
public void setPlotOnSecondAxis(boolean value)
```


Indique si cette série est tracée sur le deuxième axe des valeurs.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSecondPlotSize(short value) {#setSecondPlotSize-short-}
```
public void setSecondPlotSize(short value)
```


Renvoie ou définit la taille de la section secondaire d'un graphique « pie of pie » ou « bar of pie », exprimée en pourcentage de la taille du secteur principal. Peut être une valeur comprise entre 5 et 200.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | short |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Vrai si la série possède une ombre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowNegativeBubbles(boolean value) {#setShowNegativeBubbles-boolean-}
```
public void setShowNegativeBubbles(boolean value)
```


Vrai si les bulles négatives sont affichées pour le groupe de graphiques. Valide uniquement pour les graphiques à bulles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSizeRepresents(int value) {#setSizeRepresents-int-}
```
public void setSizeRepresents(int value)
```


Définit ce que représente la taille des bulles sur un graphique à bulles.

Voir [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea signifie que la valeur [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) correspond à la surface de la bulle. BubbleSizeRepresents.SizeIsWidth signifie que la valeur [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) correspond à la largeur de la bulle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSmooth(boolean value) {#setSmooth-boolean-}
```
public void setSmooth(boolean value)
```


Représente le lissage de courbe. Vrai si le lissage de courbe est activé pour le graphique en lignes ou le nuage de points. S'applique uniquement aux graphiques en lignes et aux nuages de points avec lignes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSplitType(int value) {#setSplitType-int-}
```
public void setSplitType(int value)
```


Renvoie ou définit une valeur qui indique comment déterminer quels points de données se trouvent dans le deuxième secteur ou la deuxième barre d’un diagramme « pie of pie » ou « bar of pie ».

Voir [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSplitValue(double value) {#setSplitValue-double-}
```
public void setSplitValue(double value)
```


Renvoie ou définit une valeur qui doit être utilisée pour déterminer quels points de données se trouvent dans le deuxième secteur ou la deuxième barre d’un diagramme « pie of pie » ou « bar of pie ».

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Définit le type d'une série de données.

Voir [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setValues(String value) {#setValues-java.lang.String-}
```
public void setValues(String value)
```


Représente les valeurs Y de cette série de graphique.

**Remarks**

Pour obtenir les valeurs réelles (correspondant à chaque point de cette série) définies par cette propriété, veuillez utiliser [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setValuesFormatCode(String value) {#setValuesFormatCode-java.lang.String-}
```
public void setValuesFormatCode(String value)
```


Représente le code de format de la liste de nombres des valeurs.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setXValues(String value) {#setXValues-java.lang.String-}
```
public void setXValues(String value)
```


Représente les valeurs X de cette série de graphique.

**Remarks**

Uniquement pour les graphiques en nuage de points et à bulles. Veuillez utiliser [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) pour les autres types de graphiques ; [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) est utilisé pour obtenir les valeurs de catégorie réelles de cette série.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setXValuesFormatCode(String value) {#setXValuesFormatCode-java.lang.String-}
```
public void setXValuesFormatCode(String value)
```


Représente le code de format de la liste de nombres des valeurs X.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

