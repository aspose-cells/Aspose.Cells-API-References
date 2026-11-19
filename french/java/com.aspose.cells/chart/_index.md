---
title: "Graphique"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente un seul graphique Excel."
type: docs
url: /fr/java/com.aspose.cells/chart/
---

**Inheritance:**
java.lang.Object
```
public class Chart
```

Encapsule l'objet qui représente un seul graphique Excel.

**Example**

Le code suivant montre comment créer un graphique avec du code .NET.

```
         Workbook workbook = new Workbook();
         	Worksheet sheet = workbook.getWorksheets().get(0);
 
         	Cells cells = sheet.getCells();
         	cells.get(0,1).putValue("Income");
         	cells.get(1,0).putValue("Company A");
         	cells.get(2,0).putValue("Company B");
         	cells.get(3,0).putValue("Company C");
         	cells.get(1,1).putValue(10000);
         	cells.get(2,1).putValue(20000);
         	cells.get(3,1).putValue(30000);
 
         	int chartIndex = sheet.getCharts().add(ChartType.COLUMN, 9, 9, 21, 15);
 
         	Chart chart = sheet.getCharts().get(chartIndex);
         chart.setChartDataRange("A1:B4", true);
         	chart.setShowLegend(true);
         	chart.getTitle().setText("Income Analysis");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [calculate()](#calculate--) | Calcule les positions personnalisées de la zone de tracé et des axes si leurs positions sont assignées automatiquement. |
| [calculate(ChartCalculateOptions calculateOptions)](#calculate-com.aspose.cells.ChartCalculateOptions-) | Calcule la position personnalisée de la zone de tracé et des axes si leur position est assignée automatiquement, avec les options de calcul du graphique. |
| [changeTemplate(byte[] data)](#changeTemplate-byte---) | Change le type de graphique avec un modèle prédéfini. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActualChartSize()](#getActualChartSize--) | Obtient la taille réelle du graphique en pixels. |
| [getActualSize()](#getActualSize--) | Obtient la taille réelle du graphique en pixels. |
| [getAutoScaling()](#getAutoScaling--) | Vrai si Microsoft Excel redimensionne un graphique 3D afin qu'il soit plus proche en taille du graphique 2D équivalent. |
| [getBackWall()](#getBackWall--) | Renvoie un objet [getWalls()](../../com.aspose.cells/chart\\#getWalls--) qui représente le mur arrière d'un graphique 3D. |
| [getCategoryAxis()](#getCategoryAxis--) | Obtient l'axe X du graphique. |
| [getChartArea()](#getChartArea--) | Obtient la zone du graphique dans la feuille de calcul. |
| [getChartDataRange()](#getChartDataRange--) | Obtient la plage source de données du graphique. |
| [getChartDataTable()](#getChartDataTable--) | Représente le tableau de données du graphique. |
| [getChartObject()](#getChartObject--) | Représente le chartShape; |
| [getChartShape()](#getChartShape--) | Représente le chartShape; |
| [getClass()](#getClass--) |  |
| [getDepthPercent()](#getDepthPercent--) | Représente la profondeur d'un graphique 3-D en pourcentage de la largeur du graphique (entre 20 et 2000 %). |
| [getDisplayNaAsBlank()](#getDisplayNaAsBlank--) | Indique s'il faut afficher \#N/A comme une valeur vide. |
| [getElevation()](#getElevation--) | Représente l'élévation de la vue du graphique 3-D, en degrés. |
| [getFilteredNSeries()](#getFilteredNSeries--) | Obtient une collection [SeriesCollection](../../com.aspose.cells/seriescollection) représentant les séries de données filtrées dans le graphique. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | Obtient l'angle de la première tranche de diagramme circulaire ou de diagramme en anneau, en degrés (dans le sens des aiguilles d'une montre à partir du vertical). |
| [getFloor()](#getFloor--) | Renvoie un objet [getFloor()](../../com.aspose.cells/chart\#getFloor--) qui représente les parois d'un graphique 3-D. |
| [getGapDepth()](#getGapDepth--) | Obtient la distance entre les séries de données dans un graphique 3-D, en pourcentage de la largeur du marqueur. |
| [getGapWidth()](#getGapWidth--) | Renvoie ou définit l'espace entre les groupes de barres ou de colonnes, en pourcentage de la largeur de la barre ou de la colonne. |
| [getHeightPercent()](#getHeightPercent--) | Renvoie ou définit la hauteur d'un graphique 3-D en pourcentage de la largeur du graphique (entre 5 et 500 %). |
| [getHidePivotFieldButtons()](#getHidePivotFieldButtons--) | Indique s'il faut masquer les boutons de champ du graphique croisé dynamique uniquement lorsque le graphique est un PivotChart. |
| [getIs3D()](#getIs3D--) | Indique si le graphique est un graphique 3D. |
| [getLegend()](#getLegend--) | Obtient la légende du graphique. |
| [getLine()](#getLine--) | Obtient la ligne. |
| [getNSeries()](#getNSeries--) | Obtient une collection [SeriesCollection](../../com.aspose.cells/seriescollection) représentant les séries de données dans le graphique. |
| [getName()](#getName--) | Obtient le nom du graphique. |
| [getPageSetup()](#getPageSetup--) | Représente la description de la mise en page dans ce graphique. |
| [getPerspective()](#getPerspective--) | Renvoie ou définit la perspective pour la vue du graphique three\\u9225\\u6178 dimensional. |
| [getPivotOptions()](#getPivotOptions--) | Spécifie les contrôles de pivot qui apparaissent sur le graphique. |
| [getPivotSource()](#getPivotSource--) | La source est les données du tableau croisé dynamique. |
| [getPlacement()](#getPlacement--) | Représente la façon dont le graphique est attaché aux cellules en dessous. |
| [getPlotArea()](#getPlotArea--) | Obtient la zone de tracé du graphique qui inclut les étiquettes des graduations des axes. |
| [getPlotBy()](#getPlotBy--) | Obtient si le tracé se fait par ligne ou colonne. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Obtient comment tracer les cellules vides. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Indique si seules les cellules visibles sont tracées. |
| [getPlotVisibleCellsOnly()](#getPlotVisibleCellsOnly--) | Indique si le tracé ne concerne que les cellules visibles. |
| [getPrintSize()](#getPrintSize--) | Obtient la taille imprimée du graphique. |
| [getRightAngleAxes()](#getRightAngleAxes--) | Vrai si les axes du graphique sont perpendiculaires. |
| [getRotationAngle()](#getRotationAngle--) | Représente la rotation de la vue du graphique 3D (la rotation de la zone de tracé autour de l'axe z, en degrés). |
| [getSecondCategoryAxis()](#getSecondCategoryAxis--) | Obtient le second axe X du graphique. |
| [getSecondValueAxis()](#getSecondValueAxis--) | Obtient le second axe Y du graphique. |
| [getSeriesAxis()](#getSeriesAxis--) | Obtient l'axe des séries du graphique. |
| [getShapes()](#getShapes--) | Renvoie toutes les formes de dessin de ce graphique. |
| [getShowDataTable()](#getShowDataTable--) | Obtient une valeur indiquant si le graphique affiche un tableau de données. |
| [getShowLegend()](#getShowLegend--) | Obtient une valeur indiquant si la légende du graphique sera affichée. |
| [getSideWall()](#getSideWall--) | Renvoie un objet [getWalls()](../../com.aspose.cells/chart\#getWalls--) qui représente la paroi latérale d'un graphique 3D. |
| [getSizeWithWindow()](#getSizeWithWindow--) | Vrai si Microsoft Excel redimensionne le graphique pour correspondre à la taille de la fenêtre de la feuille de graphique. |
| [getStyle()](#getStyle--) | Obtient le style intégré. |
| [getSubTitle()](#getSubTitle--) | Obtient le sous-titre du graphique. |
| [getTitle()](#getTitle--) | Obtient le titre du graphique. |
| [getType()](#getType--) | Obtient le type d'un graphique. |
| [getValueAxis()](#getValueAxis--) | Obtient l'axe Y du graphique. |
| [getWalls()](#getWalls--) | Renvoie un objet [getWalls()](../../com.aspose.cells/chart\#getWalls--) qui représente les parois d'un graphique 3D. |
| [getWallsAndGridlines2D()](#getWallsAndGridlines2D--) | Vrai si les lignes de grille sont dessinées en deux dimensions sur un graphique 3D. |
| [getWorksheet()](#getWorksheet--) | Obtient la feuille de calcul qui contient ce graphique. |
| [hasAxis(int aixsType, boolean isPrimary)](#hasAxis-int-boolean-) | Renvoie quels axes existent sur le graphique. |
| [hashCode()](#hashCode--) |  |
| [isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)](#isCellReferedByChart-int-int-int-) | Renvoie si la cellule référencée par le graphique. |
| [isChartDataChanged()](#isChartDataChanged--) | Détecte si la source de données d'un graphique a changé. |
| [isRectangularCornered()](#isRectangularCornered--) | Obtient une valeur indiquant si la zone du graphique a des coins rectangulaires. |
| [isReferedByChart(int rowIndex, int columnIndex)](#isReferedByChart-int-int-) | Renvoie si la cellule est référencée par le graphique. |
| [move(int topRow, int leftColumn, int bottomRow, int rightColumn)](#move-int-int-int-int-) | Déplace le graphique vers un emplacement spécifié. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshPivotData()](#refreshPivotData--) | Actualise les données du graphique à partir du tableau croisé dynamique. |
| [setAutoScaling(boolean value)](#setAutoScaling-boolean-) | Vrai si Microsoft Excel redimensionne un graphique 3D afin qu'il soit plus proche en taille du graphique 2D équivalent. |
| [setChartDataRange(String area, boolean isVertical)](#setChartDataRange-java.lang.String-boolean-) | Spécifie la plage de données pour un graphique. |
| [setDepthPercent(int value)](#setDepthPercent-int-) | Représente la profondeur d'un graphique 3-D en pourcentage de la largeur du graphique (entre 20 et 2000 %). |
| [setDisplayNaAsBlank(boolean value)](#setDisplayNaAsBlank-boolean-) | Indique s'il faut afficher \#N/A comme une valeur vide. |
| [setElevation(int value)](#setElevation-int-) | Représente l'élévation de la vue du graphique 3-D, en degrés. |
| [setFirstSliceAngle(int value)](#setFirstSliceAngle-int-) | Définit l'angle de la première tranche de diagramme circulaire ou de donut, en degrés (dans le sens des aiguilles d'une montre depuis la verticale). |
| [setGapDepth(int value)](#setGapDepth-int-) | Définit la distance entre les séries de données dans un graphique 3D, en pourcentage de la largeur du marqueur. |
| [setGapWidth(int value)](#setGapWidth-int-) | Renvoie ou définit l'espace entre les groupes de barres ou de colonnes, en pourcentage de la largeur de la barre ou de la colonne. |
| [setHeightPercent(int value)](#setHeightPercent-int-) | Renvoie ou définit la hauteur d'un graphique 3-D en pourcentage de la largeur du graphique (entre 5 et 500 %). |
| [setHidePivotFieldButtons(boolean value)](#setHidePivotFieldButtons-boolean-) | Indique s'il faut masquer les boutons de champ du graphique croisé dynamique uniquement lorsque le graphique est un PivotChart. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom du graphique. |
| [setPerspective(short value)](#setPerspective-short-) | Renvoie ou définit la perspective pour la vue du graphique three\\u9225\\u6178 dimensional. |
| [setPivotSource(String value)](#setPivotSource-java.lang.String-) | La source est les données du tableau croisé dynamique. |
| [setPlacement(int value)](#setPlacement-int-) | Représente la façon dont le graphique est attaché aux cellules en dessous. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | Définit comment tracer les cellules vides. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Indique si seules les cellules visibles sont tracées. |
| [setPlotVisibleCellsOnly(boolean value)](#setPlotVisibleCellsOnly-boolean-) | Indique si le tracé ne concerne que les cellules visibles. |
| [setPrintSize(int value)](#setPrintSize-int-) | Définit la taille imprimée du graphique. |
| [setRectangularCornered(boolean value)](#setRectangularCornered-boolean-) | Définit une valeur indiquant si la zone du graphique a des coins rectangulaires. |
| [setRightAngleAxes(boolean value)](#setRightAngleAxes-boolean-) | Vrai si les axes du graphique sont perpendiculaires. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Représente la rotation de la vue du graphique 3D (la rotation de la zone de tracé autour de l'axe z, en degrés). |
| [setShowDataTable(boolean value)](#setShowDataTable-boolean-) | Définit une valeur indiquant si le graphique affiche un tableau de données. |
| [setShowLegend(boolean value)](#setShowLegend-boolean-) | Définit une valeur indiquant si la légende du graphique sera affichée. |
| [setSizeWithWindow(boolean value)](#setSizeWithWindow-boolean-) | Vrai si Microsoft Excel redimensionne le graphique pour correspondre à la taille de la fenêtre de la feuille de graphique. |
| [setStyle(int value)](#setStyle-int-) | Définit le style intégré. |
| [setType(int value)](#setType-int-) | Définit le type d'un graphique. |
| [setWallsAndGridlines2D(boolean value)](#setWallsAndGridlines2D-boolean-) | Vrai si les lignes de grille sont dessinées en deux dimensions sur un graphique 3D. |
| [switchRowColumn()](#switchRowColumn--) | Inverse les lignes/colonnes. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Crée l'image du graphique et l'enregistre dans un flux au format spécifié. |
| [toImage(String imageFile)](#toImage-java.lang.String-) | Crée l'image du graphique et l'enregistre dans un fichier. |
| [toImage(String imageFile, ImageFormat imageFormat)](#toImage-java.lang.String-com.aspose.cells.ImageFormat-) | Crée l'image du graphique et l'enregistre dans un fichier au format spécifié. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Crée l'image du graphique et l'enregistre dans un fichier. |
| [toImage(String imageFile, int imageType)](#toImage-java.lang.String-int-) | Crée l'image du graphique et l'enregistre dans un fichier au type d'image spécifié. |
| [toImage(String imageFile, long jpegQuality)](#toImage-java.lang.String-long-) | Crée l'image du graphique et l'enregistre dans un fichier au format JPEG. |
| [toPdf(OutputStream stream)](#toPdf-java.io.OutputStream-) | Crée le PDF du graphique et l'enregistre dans un flux. |
| [toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.io.OutputStream-float-float-int-int-) | Crée le PDF du graphique et l'enregistre dans un flux. |
| [toPdf(String fileName)](#toPdf-java.lang.String-) | Enregistre le graphique dans un fichier PDF. |
| [toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.lang.String-float-float-int-int-) | Enregistre le graphique dans un fichier PDF. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate() {#calculate--}
```
public void calculate()
```


Calcule les positions personnalisées de la zone de tracé et des axes si leurs positions sont assignées automatiquement.

### calculate(ChartCalculateOptions calculateOptions) {#calculate-com.aspose.cells.ChartCalculateOptions-}
```
public void calculate(ChartCalculateOptions calculateOptions)
```


Calcule la position personnalisée de la zone de tracé et des axes si leur position est assignée automatiquement, avec les options de calcul du graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| calculateOptions | [ChartCalculateOptions](../../com.aspose.cells/chartcalculateoptions) |  |

### changeTemplate(byte[] data) {#changeTemplate-byte---}
```
public void changeTemplate(byte[] data)
```


Change le type de graphique avec un modèle prédéfini.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| données | byte[] | Les données du fichier de modèle de graphique (.crtx). |

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
### getActualChartSize() {#getActualChartSize--}
```
public int[] getActualChartSize()
```


Obtient la taille réelle du graphique en pixels.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Chart.getActualSize(). Cette propriété sera supprimée 12 mois plus tard, à compter de juillet 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int[] - Taille réelle dans un tableau (largeur et hauteur). [0] est la largeur ; [1] est la hauteur.
### getActualSize() {#getActualSize--}
```
public int[] getActualSize()
```


Obtient la taille réelle du graphique en pixels.

**Returns:**
int[] - Taille réelle dans un tableau (largeur et hauteur). [0] est la largeur ; [1] est la hauteur.
### getAutoScaling() {#getAutoScaling--}
```
public boolean getAutoScaling()
```


Vrai si Microsoft Excel redimensionne un graphique 3‑D afin qu’il soit plus proche en taille du graphique 2‑D équivalent. La propriété RightAngleAxes doit être vraie.

**Returns:**
boolean
### getBackWall() {#getBackWall--}
```
public Walls getBackWall()
```


Renvoie un objet [getWalls()](../../com.aspose.cells/chart\\#getWalls--) qui représente le mur arrière d'un graphique 3D.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getCategoryAxis() {#getCategoryAxis--}
```
public Axis getCategoryAxis()
```


Obtient l'axe X du graphique.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getChartArea() {#getChartArea--}
```
public ChartArea getChartArea()
```


Obtient la zone du graphique dans la feuille de calcul.

**Returns:**
[ChartArea](../../com.aspose.cells/chartarea)
### getChartDataRange() {#getChartDataRange--}
```
public String getChartDataRange()
```


Obtient la plage source de données du graphique.

**Remarks**

Ne prend en charge que les plages. Si les propriétés Series.Values, Name et XValues se trouvent dans une plage continue, une plage les contenant sera renvoyée.

**Returns:**
java.lang.String - La source de données.
### getChartDataTable() {#getChartDataTable--}
```
public ChartDataTable getChartDataTable()
```


Représente le tableau de données du graphique.

**Returns:**
[ChartDataTable](../../com.aspose.cells/chartdatatable)
### getChartObject() {#getChartObject--}
```
public ChartShape getChartObject()
```


Représente le chartShape;

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getChartShape() {#getChartShape--}
```
public ChartShape getChartShape()
```


Représente le chartShape;

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Aspose.Cells.Charts.Chart.ChartObject. Cette propriété sera supprimée 12 mois plus tard, à compter de janvier 2012. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDepthPercent() {#getDepthPercent--}
```
public int getDepthPercent()
```


Représente la profondeur d'un graphique 3-D en pourcentage de la largeur du graphique (entre 20 et 2000 %).

**Returns:**
int
### getDisplayNaAsBlank() {#getDisplayNaAsBlank--}
```
public boolean getDisplayNaAsBlank()
```


Indique s'il faut afficher \#N/A comme une valeur vide.

**Returns:**
boolean
### getElevation() {#getElevation--}
```
public int getElevation()
```


Représente l'élévation de la vue du graphique 3-D, en degrés.

**Remarks**

L’élévation du graphique est la hauteur à laquelle vous visualisez le graphique, en degrés. La valeur par défaut est 15 pour la plupart des types de graphiques. La valeur de cette propriété doit être comprise entre -90 et 90, sauf pour les graphiques à barres 3‑D, où elle doit être comprise entre 0 et 44.

**Returns:**
int
### getFilteredNSeries() {#getFilteredNSeries--}
```
public SeriesCollection getFilteredNSeries()
```


Obtient une collection [SeriesCollection](../../com.aspose.cells/seriescollection) représentant les séries de données filtrées dans le graphique.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public int getFirstSliceAngle()
```


Obtient l’angle de la première tranche de diagramme circulaire ou de beignet, en degrés (dans le sens des aiguilles d’une montre à partir du vertical). S’applique uniquement aux diagrammes circulaires, aux diagrammes circulaires 3‑D et aux diagrammes beignet, de 0 à 360.

**Returns:**
int
### getFloor() {#getFloor--}
```
public Floor getFloor()
```


Renvoie un objet [getFloor()](../../com.aspose.cells/chart\#getFloor--) qui représente les parois d'un graphique 3-D.

**Remarks**

Cette propriété ne s’applique pas aux diagrammes circulaires 3‑D.

**Returns:**
[Floor](../../com.aspose.cells/floor)
### getGapDepth() {#getGapDepth--}
```
public int getGapDepth()
```


Obtient la distance entre les séries de données dans un graphique 3‑D, exprimée en pourcentage de la largeur du marqueur. La valeur de cette propriété doit être comprise entre 0 et 500.

**Returns:**
int
### getGapWidth() {#getGapWidth--}
```
public int getGapWidth()
```


Renvoie ou définit l’espace entre les groupes de barres ou de colonnes, exprimé en pourcentage de la largeur de la barre ou de la colonne. La valeur de cette propriété doit être comprise entre 0 et 500.

**Returns:**
int
### getHeightPercent() {#getHeightPercent--}
```
public int getHeightPercent()
```


Renvoie ou définit la hauteur d'un graphique 3-D en pourcentage de la largeur du graphique (entre 5 et 500 %).

**Returns:**
int
### getHidePivotFieldButtons() {#getHidePivotFieldButtons--}
```
public boolean getHidePivotFieldButtons()
```


Indique s'il faut masquer les boutons de champ du graphique croisé dynamique uniquement lorsque le graphique est un PivotChart.

**Returns:**
boolean
### getIs3D() {#getIs3D--}
```
public boolean getIs3D()
```


Indique si le graphique est un graphique 3D.

**Returns:**
boolean
### getLegend() {#getLegend--}
```
public Legend getLegend()
```


Obtient la légende du graphique.

**Returns:**
[Legend](../../com.aspose.cells/legend)
### getLine() {#getLine--}
```
public Line getLine()
```


Obtient la ligne.

**Returns:**
[Line](../../com.aspose.cells/line)
### getNSeries() {#getNSeries--}
```
public SeriesCollection getNSeries()
```


Obtient une collection [SeriesCollection](../../com.aspose.cells/seriescollection) représentant les séries de données dans le graphique.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getName() {#getName--}
```
public String getName()
```


Obtient le nom du graphique.

**Returns:**
java.lang.String
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


Représente la description de la mise en page dans ce graphique.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPerspective() {#getPerspective--}
```
public short getPerspective()
```


Renvoie ou définit la perspective pour la vue du graphique tridimensionnel three\\u9225\\u6178. Doit être comprise entre 0 et 100. Cette propriété est ignorée si la propriété RightAngleAxes est vraie.

**Returns:**
short
### getPivotOptions() {#getPivotOptions--}
```
public PivotOptions getPivotOptions()
```


Spécifie les contrôles de pivot qui apparaissent sur le graphique.

**Returns:**
[PivotOptions](../../com.aspose.cells/pivotoptions)
### getPivotSource() {#getPivotSource--}
```
public String getPivotSource()
```


La source est les données du tableau croisé dynamique. Si PivotSource n’est pas vide, le graphique est un PivotChart.

**Remarks**

Si le tableau croisé dynamique "PivotTable1" se trouve dans la feuille de calcul "Sheet1" du fichier "Book1.xls". Le pivotSource pourrait être "[Book1.xls]Sheet1!PivotTable1" si le graphique et le tableau croisé dynamique ne sont pas dans le même classeur. Si vous définissez cette propriété, le paramètre de source de données précédent sera perdu.

**Returns:**
java.lang.String
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Représente la façon dont le graphique est attaché aux cellules en dessous.

Voir [PlacementType](../../com.aspose.cells/placementtype).

**Returns:**
int
### getPlotArea() {#getPlotArea--}
```
public PlotArea getPlotArea()
```


Obtient la zone de tracé du graphique qui inclut les étiquettes des graduations des axes.

**Remarks**

**Returns:**
[PlotArea](../../com.aspose.cells/plotarea)
### getPlotBy() {#getPlotBy--}
```
public int getPlotBy()
```


Obtient si le tracé se fait par ligne ou colonne.

Voir [PlotDataByType](../../com.aspose.cells/plotdatabytype).

**Returns:**
int
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


Obtient comment tracer les cellules vides.

Voir [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


Indique si seules les cellules visibles sont tracées.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété PlotVisibleCellsOnly. Cette méthode sera supprimée 12 mois plus tard, à compter de décembre 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### getPlotVisibleCellsOnly() {#getPlotVisibleCellsOnly--}
```
public boolean getPlotVisibleCellsOnly()
```


Indique si le tracé ne concerne que les cellules visibles.

**Returns:**
boolean
### getPrintSize() {#getPrintSize--}
```
public int getPrintSize()
```


Obtient la taille imprimée du graphique.

Voir [PrintSizeType](../../com.aspose.cells/printsizetype).

**Returns:**
int
### getRightAngleAxes() {#getRightAngleAxes--}
```
public boolean getRightAngleAxes()
```


Vrai si les axes du graphique sont à angle droit. S’applique uniquement aux graphiques 3‑D (excepté Column3D et les graphiques circulaires 3‑D).

**Remarks**

Si cette propriété est vraie, la propriété Perspective est ignorée.

**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Représente la rotation de la vue du graphique 3D (la rotation de la zone de tracé autour de l'axe z, en degrés).

**Remarks**

La valeur de cette propriété doit être comprise entre 0 et 360, sauf pour les graphiques à barres 3‑D, où elle doit être comprise entre 0 et 44. La valeur par défaut est 20. S’applique uniquement aux graphiques 3‑D.

**Returns:**
int
### getSecondCategoryAxis() {#getSecondCategoryAxis--}
```
public Axis getSecondCategoryAxis()
```


Obtient le second axe X du graphique.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSecondValueAxis() {#getSecondValueAxis--}
```
public Axis getSecondValueAxis()
```


Obtient le second axe Y du graphique.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSeriesAxis() {#getSeriesAxis--}
```
public Axis getSeriesAxis()
```


Obtient l'axe des séries du graphique.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


Renvoie toutes les formes de dessin de ce graphique.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTable() {#getShowDataTable--}
```
public boolean getShowDataTable()
```


Obtient une valeur indiquant si le graphique affiche un tableau de données.

**Returns:**
boolean
### getShowLegend() {#getShowLegend--}
```
public boolean getShowLegend()
```


Obtient une valeur indiquant si la légende du graphique sera affichée. La valeur par défaut est vraie.

**Returns:**
boolean
### getSideWall() {#getSideWall--}
```
public Walls getSideWall()
```


Renvoie un objet [getWalls()](../../com.aspose.cells/chart\#getWalls--) qui représente la paroi latérale d'un graphique 3D.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getSizeWithWindow() {#getSizeWithWindow--}
```
public boolean getSizeWithWindow()
```


Vrai si Microsoft Excel redimensionne le graphique pour correspondre à la taille de la fenêtre de la feuille de graphique.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public int getStyle()
```


Obtient le style intégré.

**Remarks**

Elle doit être comprise entre 1 et 48. Retourne -1 si elle n’est pas définie.

**Returns:**
int
### getSubTitle() {#getSubTitle--}
```
public Title getSubTitle()
```


Obtient le sous-titre du graphique. S’applique uniquement aux fichiers ODS.

**Returns:**
[Title](../../com.aspose.cells/title)
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Obtient le titre du graphique.

**Returns:**
[Title](../../com.aspose.cells/title)
### getType() {#getType--}
```
public int getType()
```


Obtient le type d'un graphique.

Voir [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getValueAxis() {#getValueAxis--}
```
public Axis getValueAxis()
```


Obtient l'axe Y du graphique.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getWalls() {#getWalls--}
```
public Walls getWalls()
```


Renvoie un objet [getWalls()](../../com.aspose.cells/chart\#getWalls--) qui représente les parois d'un graphique 3D.

**Remarks**

Cette propriété ne s’applique pas aux diagrammes circulaires 3‑D.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getWallsAndGridlines2D() {#getWallsAndGridlines2D--}
```
public boolean getWallsAndGridlines2D()
```


Vrai si les lignes de grille sont dessinées en deux dimensions sur un graphique 3D.

**Returns:**
boolean
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Obtient la feuille de calcul qui contient ce graphique.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasAxis(int aixsType, boolean isPrimary) {#hasAxis-int-boolean-}
```
public boolean hasAxis(int aixsType, boolean isPrimary)
```


Renvoie quels axes existent sur le graphique.

**Remarks**

Normalement, Pie, PieExploded, PiePie,PieBar, Pie3D, Pie3DExploded,Doughnut, DoughnutExploded n'ont pas d'axe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| aixsType | int |  |
| isPrimary | boolean |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex) {#isCellReferedByChart-int-int-int-}
```
public boolean isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)
```


Renvoie si la cellule référencée par le graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | int | L'index de la feuille -1 signifie la feuille de calcul qui contient le graphique actuel. |
| rowIndex | int | L'index de ligne |
| columnIndex | int | L'index de colonne |

**Returns:**
boolean -
### isChartDataChanged() {#isChartDataChanged--}
```
public boolean isChartDataChanged()
```


Détecte si la source de données d'un graphique a changé.

**Remarks**

La méthode détecte les modifications de la source de données du graphique avant de rendre le graphique au format image. Lors du premier appel à Chart.toImage, les données sources du graphique (par ex. XValuesParseData, ValuesParseData) seront enregistrées. Avant d'appeler à nouveau la méthode Chart.toImage, appelez la méthode IsChartDataChanged pour vérifier si le graphique doit être re‑rendu.

**Returns:**
booléen - Retourne true si le graphique a changé, sinon retourne false
### isRectangularCornered() {#isRectangularCornered--}
```
public boolean isRectangularCornered()
```


Obtient une valeur indiquant si la zone du graphique a des coins rectangulaires. La valeur par défaut est true.

**Returns:**
boolean
### isReferedByChart(int rowIndex, int columnIndex) {#isReferedByChart-int-int-}
```
public boolean isReferedByChart(int rowIndex, int columnIndex)
```


Renvoie si la cellule est référencée par le graphique.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode IsCellReferedByChart(int,int,int). Cette méthode sera supprimée 12 mois plus tard, à compter d'avril 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | L'index de ligne |
| columnIndex | int | L'index de colonne |

**Returns:**
boolean -
### move(int topRow, int leftColumn, int bottomRow, int rightColumn) {#move-int-int-int-int-}
```
public void move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Déplace le graphique vers un emplacement spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| bottomRow | int | Indice de ligne en bas à droite |
| rightColumn | int | Indice de colonne en bas à droite |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshPivotData() {#refreshPivotData--}
```
public void refreshPivotData()
```


Actualise les données du graphique à partir du tableau croisé dynamique.

**Remarks**

Nous recueillerons les données de la source de données pivot vers le rapport de tableau croisé dynamique. Cette méthode n'est utilisée que pour rassembler toutes les données vers un graphique pivot.

### setAutoScaling(boolean value) {#setAutoScaling-boolean-}
```
public void setAutoScaling(boolean value)
```


Vrai si Microsoft Excel redimensionne un graphique 3‑D afin qu’il soit plus proche en taille du graphique 2‑D équivalent. La propriété RightAngleAxes doit être vraie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setChartDataRange(String area, boolean isVertical) {#setChartDataRange-java.lang.String-boolean-}
```
public void setChartDataRange(String area, boolean isVertical)
```


Spécifie la plage de données pour un graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| area | java.lang.String | Spécifie les valeurs à partir desquelles tracer la série de données |
| isVertical | boolean | Spécifie si la série doit être tracée à partir d'une plage de valeurs de cellules par ligne ou par colonne. |

### setDepthPercent(int value) {#setDepthPercent-int-}
```
public void setDepthPercent(int value)
```


Représente la profondeur d'un graphique 3-D en pourcentage de la largeur du graphique (entre 20 et 2000 %).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDisplayNaAsBlank(boolean value) {#setDisplayNaAsBlank-boolean-}
```
public void setDisplayNaAsBlank(boolean value)
```


Indique s'il faut afficher \#N/A comme une valeur vide.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setElevation(int value) {#setElevation-int-}
```
public void setElevation(int value)
```


Représente l'élévation de la vue du graphique 3-D, en degrés.

**Remarks**

L’élévation du graphique est la hauteur à laquelle vous visualisez le graphique, en degrés. La valeur par défaut est 15 pour la plupart des types de graphiques. La valeur de cette propriété doit être comprise entre -90 et 90, sauf pour les graphiques à barres 3‑D, où elle doit être comprise entre 0 et 44.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setFirstSliceAngle(int value) {#setFirstSliceAngle-int-}
```
public void setFirstSliceAngle(int value)
```


Définit l'angle de la première tranche de diagramme circulaire ou de diagramme en anneau, en degrés (dans le sens des aiguilles d'une montre à partir du vertical). S'applique uniquement aux diagrammes circulaires, 3D circulaires et en anneau, de 0 à 360.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setGapDepth(int value) {#setGapDepth-int-}
```
public void setGapDepth(int value)
```


Définit la distance entre les séries de données dans un graphique 3D, en pourcentage de la largeur du marqueur. La valeur de cette propriété doit être comprise entre 0 et 500.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setGapWidth(int value) {#setGapWidth-int-}
```
public void setGapWidth(int value)
```


Renvoie ou définit l’espace entre les groupes de barres ou de colonnes, exprimé en pourcentage de la largeur de la barre ou de la colonne. La valeur de cette propriété doit être comprise entre 0 et 500.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHeightPercent(int value) {#setHeightPercent-int-}
```
public void setHeightPercent(int value)
```


Renvoie ou définit la hauteur d'un graphique 3-D en pourcentage de la largeur du graphique (entre 5 et 500 %).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHidePivotFieldButtons(boolean value) {#setHidePivotFieldButtons-boolean-}
```
public void setHidePivotFieldButtons(boolean value)
```


Indique s'il faut masquer les boutons de champ du graphique croisé dynamique uniquement lorsque le graphique est un PivotChart.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Définit le nom du graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPerspective(short value) {#setPerspective-short-}
```
public void setPerspective(short value)
```


Renvoie ou définit la perspective pour la vue du graphique tridimensionnel three\\u9225\\u6178. Doit être comprise entre 0 et 100. Cette propriété est ignorée si la propriété RightAngleAxes est vraie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | short |  |

### setPivotSource(String value) {#setPivotSource-java.lang.String-}
```
public void setPivotSource(String value)
```


La source est les données du tableau croisé dynamique. Si PivotSource n’est pas vide, le graphique est un PivotChart.

**Remarks**

Si le tableau croisé dynamique "PivotTable1" se trouve dans la feuille de calcul "Sheet1" du fichier "Book1.xls". Le pivotSource pourrait être "[Book1.xls]Sheet1!PivotTable1" si le graphique et le tableau croisé dynamique ne sont pas dans le même classeur. Si vous définissez cette propriété, le paramètre de source de données précédent sera perdu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Représente la façon dont le graphique est attaché aux cellules en dessous.

Voir [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


Définit comment tracer les cellules vides.

Voir [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


Indique si seules les cellules visibles sont tracées.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété PlotVisibleCellsOnly. Cette méthode sera supprimée 12 mois plus tard, à compter de décembre 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPlotVisibleCellsOnly(boolean value) {#setPlotVisibleCellsOnly-boolean-}
```
public void setPlotVisibleCellsOnly(boolean value)
```


Indique si le tracé ne concerne que les cellules visibles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPrintSize(int value) {#setPrintSize-int-}
```
public void setPrintSize(int value)
```


Définit la taille imprimée du graphique.

Voir [PrintSizeType](../../com.aspose.cells/printsizetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRectangularCornered(boolean value) {#setRectangularCornered-boolean-}
```
public void setRectangularCornered(boolean value)
```


Définit une valeur indiquant si la zone du graphique a des coins rectangulaires. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRightAngleAxes(boolean value) {#setRightAngleAxes-boolean-}
```
public void setRightAngleAxes(boolean value)
```


Vrai si les axes du graphique sont à angle droit. S’applique uniquement aux graphiques 3‑D (excepté Column3D et les graphiques circulaires 3‑D).

**Remarks**

Si cette propriété est vraie, la propriété Perspective est ignorée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Représente la rotation de la vue du graphique 3D (la rotation de la zone de tracé autour de l'axe z, en degrés).

**Remarks**

La valeur de cette propriété doit être comprise entre 0 et 360, sauf pour les graphiques à barres 3‑D, où elle doit être comprise entre 0 et 44. La valeur par défaut est 20. S’applique uniquement aux graphiques 3‑D.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setShowDataTable(boolean value) {#setShowDataTable-boolean-}
```
public void setShowDataTable(boolean value)
```


Définit une valeur indiquant si le graphique affiche un tableau de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowLegend(boolean value) {#setShowLegend-boolean-}
```
public void setShowLegend(boolean value)
```


Définit une valeur indiquant si la légende du graphique sera affichée. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSizeWithWindow(boolean value) {#setSizeWithWindow-boolean-}
```
public void setSizeWithWindow(boolean value)
```


Vrai si Microsoft Excel redimensionne le graphique pour correspondre à la taille de la fenêtre de la feuille de graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


Définit le style intégré.

**Remarks**

Elle doit être comprise entre 1 et 48. Retourne -1 si elle n’est pas définie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Définit le type d'un graphique.

Voir [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setWallsAndGridlines2D(boolean value) {#setWallsAndGridlines2D-boolean-}
```
public void setWallsAndGridlines2D(boolean value)
```


Vrai si les lignes de grille sont dessinées en deux dimensions sur un graphique 3D.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### switchRowColumn() {#switchRowColumn--}
```
public boolean switchRowColumn()
```


Inverse les lignes/colonnes.

**Returns:**
booléen - False signifie que le basculement ligne/colonne échoue.
### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Crée l'image du graphique et l'enregistre dans un flux au format spécifié.

**Remarks**

Le format de l'image est spécifié en utilisant `options.ImageFormat`. Les formats suivants sont pris en charge : ImageFormat.Bmp, ImageFormat.Gif, ImageFormat.Png, ImageFormat.Jpeg, ImageFormat.Tiff, ImageFormat.Emf.

Si la largeur ou la hauteur est zéro ou si le graphique n'est pas pris en charge selon la Liste des graphiques pris en charge, cette méthode ne fera rien. Veuillez vous référer à [Supported Charts List][] pour plus de détails.


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux de sortie. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Options supplémentaires de création d'image |

### toImage(String imageFile) {#toImage-java.lang.String-}
```
public void toImage(String imageFile)
```


Crée l'image du graphique et l'enregistre dans un fichier. L'extension du nom de fichier détermine le format de l'image.

**Remarks**

Le format de l'image est spécifié en utilisant l'extension du nom de fichier. Par exemple, si vous spécifiez "myfile.png", l'image sera enregistrée au format PNG. Les extensions de fichier suivantes sont reconnues : .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Si la largeur ou la hauteur est zéro ou si le graphique n'est pas pris en charge selon la Liste des graphiques pris en charge, cette méthode ne fera rien.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| imageFile | java.lang.String | Le nom du fichier image avec le chemin complet. |

### toImage(String imageFile, ImageFormat imageFormat) {#toImage-java.lang.String-com.aspose.cells.ImageFormat-}
```
public void toImage(String imageFile, ImageFormat imageFormat)
```


Crée l'image du graphique et l'enregistre dans un fichier au format spécifié.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Chart.ToImage(string, ImageType). Cette propriété sera supprimée 12 mois plus tard, à compter de juillet 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| imageFile | java.lang.String | Le nom du fichier image avec le chemin complet. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | Le format dans lequel enregistrer l'image. |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


Crée l'image du graphique et l'enregistre dans un fichier. L'extension du nom de fichier détermine le format de l'image.

**Remarks**

Le format de l'image est spécifié en utilisant l'extension du nom de fichier. Par exemple, si vous spécifiez "myfile.png", l'image sera enregistrée au format PNG. Les extensions de fichier suivantes sont reconnues : .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Si la largeur ou la hauteur est zéro ou si le graphique n'est pas pris en charge selon la Liste des graphiques pris en charge, cette méthode ne fera rien. Veuillez vous référer à [Supported Charts List][] pour plus de détails.

**Example**

Enregistre au format Tiff avec 300 dpi et compression CCITT4.

```
         ImageOrPrintOptions options = new ImageOrPrintOptions();
         options.setHorizontalResolution(300);
         options.setVerticalResolution(300);
         options.setTiffCompression(TiffCompression.COMPRESSION_CCITT_4);
 
         Workbook book = new Workbook("test.xls");
         book.getWorksheets().get(0).getCharts().get(0).toImage("chart.Tiff", options);
```


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| imageFile | java.lang.String | Le nom du fichier image avec le chemin complet. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Options supplémentaires de création d'image |

### toImage(String imageFile, int imageType) {#toImage-java.lang.String-int-}
```
public void toImage(String imageFile, int imageType)
```


Crée l'image du graphique et l'enregistre dans un fichier au type d'image spécifié.

**Remarks**

Le type de l'image est spécifié en utilisant `imageType`. Les types suivants sont pris en charge : ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Si la largeur ou la hauteur est zéro ou si le graphique n'est pas pris en charge selon la Liste des graphiques pris en charge, cette méthode ne fera rien.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| imageFile | java.lang.String | Le nom du fichier image avec le chemin complet. |
| imageType | int | [ImageType](../../com.aspose.cells/imagetype). Le type d'image dans lequel enregistrer l'image. |

### toImage(String imageFile, long jpegQuality) {#toImage-java.lang.String-long-}
```
public void toImage(String imageFile, long jpegQuality)
```


Crée l'image du graphique et l'enregistre dans un fichier au format JPEG.

**Remarks**

Si la largeur ou la hauteur est zéro ou si le graphique n'est pas pris en charge selon la Liste des graphiques pris en charge, cette méthode ne fera rien. NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode ToImage(string,ImageOrPrintOptions) avec la qualité spécifiée. Cette méthode sera supprimée 12 mois plus tard, à compter de mars 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| imageFile | java.lang.String | Le nom du fichier image avec le chemin complet. |
| jpegQuality | long | Qualité JPEG. |

### toPdf(OutputStream stream) {#toPdf-java.io.OutputStream-}
```
public void toPdf(OutputStream stream)
```


Crée le PDF du graphique et l'enregistre dans un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux de sortie. |

### toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.io.OutputStream-float-float-int-int-}
```
public void toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


Crée le PDF du graphique et l'enregistre dans un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux de sortie. |
| desiredPageWidth | float | La largeur de page souhaitée en pouces. |
| desiredPageHeight | float | La hauteur de page souhaitée en pouces. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Le type d'alignement horizontal du graphique dans la page de sortie. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Le type d'alignement vertical du graphique dans la page de sortie. |

### toPdf(String fileName) {#toPdf-java.lang.String-}
```
public void toPdf(String fileName)
```


Enregistre le graphique dans un fichier PDF.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | le nom du fichier PDF avec le chemin complet |

### toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.lang.String-float-float-int-int-}
```
public void toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


Enregistre le graphique dans un fichier PDF.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | le nom du fichier PDF avec le chemin complet |
| desiredPageWidth | float | La largeur de page souhaitée en pouces. |
| desiredPageHeight | float | La hauteur de page souhaitée en pouces. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Le type d'alignement horizontal du graphique dans la page de sortie. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Le type d'alignement vertical du graphique dans la page de sortie. |

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

