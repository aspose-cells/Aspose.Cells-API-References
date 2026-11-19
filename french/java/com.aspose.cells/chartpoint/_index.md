---
title: "ChartPoint"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un point unique dans une série d'un graphique."
type: docs
url: /fr/java/com.aspose.cells/chartpoint/
---

**Inheritance:**
java.lang.Object
```
public class ChartPoint
```

Représente un point unique dans une série d'un graphique.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
 
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
 
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
 
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
 
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
 
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
 
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.PIE_EXPLODED, 5, 0, 25, 10);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         //Show Data Labels 
         chart.getNSeries().get(0).getDataLabels().setShowValue(true);
 
         for (int i = 0; i  <chart.getNSeries().get(0).getPoints().getCount(); i++)
         {
             //Get Data Point
             ChartPoint point = chart.getNSeries().get(0).getPoints().get(i);
             //Set Pir Explosion
             point.setExplosion(15);
             //Set Border Color
             point.getBorder().setColor(com.aspose.cells.Color.getRed());
         }
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArcEndPointXPx()](#getArcEndPointXPx--) | Obtient la coordonnée x du point final de la section du secteur après avoir appelé la méthode Chart.Calculate(). |
| [getArcEndPointYPx()](#getArcEndPointYPx--) | Obtient la coordonnée y du point final de la section du secteur après avoir appelé la méthode Chart.Calculate(). |
| [getArcStartPointXPx()](#getArcStartPointXPx--) | Obtient la coordonnée x du point de départ de la section du diagramme circulaire après l'appel de la méthode Chart.Calculate(). |
| [getArcStartPointYPx()](#getArcStartPointYPx--) | Obtient la coordonnée y du point de départ de la section du diagramme circulaire après l'appel de la méthode Chart.Calculate(). |
| [getArea()](#getArea--) | Obtient le [getArea()](../../com.aspose.cells/chartpoint\#getArea--). |
| [getBorder()](#getBorder--) | Obtient le [Line](../../com.aspose.cells/line). |
| [getBorderWidthPx()](#getBorderWidthPx--) | Obtient la largeur de la bordure en pixels après l'appel de la méthode Chart.Calculate(). |
| [getBottomPointCount()](#getBottomPointCount--) | Obtient le nombre de points inférieurs après l'appel de la méthode Chart.Calculate(). |
| [getBottomPointXPx(int index)](#getBottomPointXPx-int-) | Obtient la coordonnée x du point inférieur de la forme après l'appel de la méthode Chart.Calculate(). |
| [getBottomPointYPx(int index)](#getBottomPointYPx-int-) | Obtient la coordonnée y du point inférieur de la forme après l'appel de la méthode Chart.Calculate(). |
| [getClass()](#getClass--) |  |
| [getDataLabels()](#getDataLabels--) | Renvoie un objet [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) qui représente l'étiquette de données associée à ce point de graphique. |
| [getDoughnutInnerRadius()](#getDoughnutInnerRadius--) | Obtient le rayon interne de la tranche de beignet en pixels après l'appel de la méthode Chart.Calculate(). |
| [getEndAngle()](#getEndAngle--) | Obtient l'angle final de la section du diagramme circulaire, mesuré en degrés dans le sens horaire à partir de l'axe x après l'appel de la méthode Chart.Calculate(). |
| [getExplosion()](#getExplosion--) | La distance d'une tranche de diagramme circulaire ouverte du centre du diagramme circulaire est exprimée en pourcentage du diamètre du diagramme. |
| [getInnerArcEndPointXPx()](#getInnerArcEndPointXPx--) | Obtient la coordonnée x du point final de la section du secteur après avoir appelé la méthode Chart.Calculate(). |
| [getInnerArcEndPointYPx()](#getInnerArcEndPointYPx--) | Obtient la coordonnée y du point final de la section du secteur après avoir appelé la méthode Chart.Calculate(). |
| [getInnerArcStartPointXPx()](#getInnerArcStartPointXPx--) | Obtient la coordonnée x du point de départ de la section du diagramme circulaire après l'appel de la méthode Chart.Calculate(). |
| [getInnerArcStartPointYPx()](#getInnerArcStartPointYPx--) | Obtient la coordonnée y du point de départ de la section du diagramme circulaire après l'appel de la méthode Chart.Calculate(). |
| [getInnerRadiusPx()](#getInnerRadiusPx--) | Obtient le rayon interne de la tranche de beignet en pixels après l'appel de la méthode Chart.Calculate(). |
| [getMarker()](#getMarker--) | Obtient le [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--). |
| [getOnCategoryAxisPointCount()](#getOnCategoryAxisPointCount--) | Obtient le nombre de points sur l'axe des catégories après l'appel de la méthode Chart.Calculate(). |
| [getOnCategoryAxisPointXPx(int index)](#getOnCategoryAxisPointXPx-int-) | Obtient la coordonnée x du point sur l'axe des catégories après l'appel de la méthode Chart.Calculate(). |
| [getOnCategoryAxisPointYPx(int index)](#getOnCategoryAxisPointYPx-int-) | Obtient la coordonnée y du point sur l'axe des catégories après l'appel de la méthode Chart.Calculate(). |
| [getRadiusPx()](#getRadiusPx--) | Obtient le rayon de la bulle, du diagramme circulaire ou du beignet en pixels après l'appel de la méthode Chart.Calculate(). |
| [getShadow()](#getShadow--) | Vrai si le point de graphique possède une ombre. |
| [getShapeHeight()](#getShapeHeight--) | Obtient la hauteur en unités de 1/4000 de la hauteur du graphique après l'appel de la méthode Chart.Calculate(). |
| [getShapeHeightPx()](#getShapeHeightPx--) | Obtient la hauteur en pixels après l'appel de la méthode Chart.Calculate(). |
| [getShapeProperties()](#getShapeProperties--) | Obtient l'objet [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) qui contient les propriétés visuelles de forme du ChartPoint. |
| [getShapeWidth()](#getShapeWidth--) | Obtient la largeur en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate(). |
| [getShapeWidthPx()](#getShapeWidthPx--) | Obtient la largeur en pixels après l'appel de la méthode Chart.Calculate(). |
| [getShapeX()](#getShapeX--) | Obtient la coordonnée x du coin supérieur gauche en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate(). |
| [getShapeXPx()](#getShapeXPx--) | Obtient la coordonnée x du coin supérieur gauche en pixels après l'appel de la méthode Chart.Calculate(). |
| [getShapeY()](#getShapeY--) | Obtient la coordonnée y du coin supérieur gauche en unités de 1/4000 de la hauteur du graphique après l'appel de la méthode Chart.Calculate(). |
| [getShapeYPx()](#getShapeYPx--) | Obtient la coordonnée y du coin supérieur gauche en pixels après l'appel de la méthode Chart.Calculate(). |
| [getStartAngle()](#getStartAngle--) | Obtient l'angle de départ de la section du camembert, mesuré en degrés dans le sens horaire à partir de l'axe x après l'appel de la méthode Chart.Calculate(). |
| [getTopPointCount()](#getTopPointCount--) | Obtient le nombre de points supérieurs après l'appel de la méthode Chart.Calculate(). |
| [getTopPointXPx(int index)](#getTopPointXPx-int-) | Obtient la coordonnée x du point supérieur de la forme après l'appel de la méthode Chart.Calculate(). |
| [getTopPointYPx(int index)](#getTopPointYPx-int-) | Obtient la coordonnée y du point supérieur de la forme après l'appel de la méthode Chart.Calculate(). |
| [getXValue()](#getXValue--) | Obtient la valeur X du point du graphique. |
| [getXValueType()](#getXValueType--) | Obtient le type de valeur X du point du graphique. |
| [getYValue()](#getYValue--) | Obtient la valeur Y du point du graphique. |
| [getYValueType()](#getYValueType--) | Obtient le type de valeur Y du point du graphique. |
| [hashCode()](#hashCode--) |  |
| [isInSecondaryPlot()](#isInSecondaryPlot--) | Obtient une valeur indiquant si ce point de données se trouve dans le deuxième camembert ou barre d'un graphique en camembert de camembert ou barre de camembert. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExplosion(int value)](#setExplosion-int-) | La distance d'une tranche de diagramme circulaire ouverte du centre du diagramme circulaire est exprimée en pourcentage du diamètre du diagramme. |
| [setInSecondaryPlot(boolean value)](#setInSecondaryPlot-boolean-) | Définit une valeur indiquant si ce point de données se trouve dans le deuxième camembert ou barre d'un graphique en camembert de camembert ou barre de camembert. |
| [setShadow(boolean value)](#setShadow-boolean-) | Vrai si le point de graphique possède une ombre. |
| [setXValue(Object value)](#setXValue-java.lang.Object-) | Définit la valeur X du point du graphique. |
| [setYValue(Object value)](#setYValue-java.lang.Object-) | Définit la valeur Y du point du graphique. |
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
### getArcEndPointXPx() {#getArcEndPointXPx--}
```
public float getArcEndPointXPx()
```


Obtient la coordonnée x du point final de la section du camembert après l'appel de la méthode Chart.Calculate(). S'applique aux graphiques Pie et Doughnut.

**Returns:**
float
### getArcEndPointYPx() {#getArcEndPointYPx--}
```
public float getArcEndPointYPx()
```


Obtient la coordonnée y du point final de la section du camembert après l'appel de la méthode Chart.Calculate(). S'applique aux graphiques Pie et Doughnut.

**Returns:**
float
### getArcStartPointXPx() {#getArcStartPointXPx--}
```
public float getArcStartPointXPx()
```


Obtient la coordonnée x du point de départ de la section du camembert après l'appel de la méthode Chart.Calculate(). S'applique aux graphiques Pie et Doughnut.

**Returns:**
float
### getArcStartPointYPx() {#getArcStartPointYPx--}
```
public float getArcStartPointYPx()
```


Obtient la coordonnée y du point de départ de la section du camembert après l'appel de la méthode Chart.Calculate(). S'applique aux graphiques Pie et Doughnut.

**Returns:**
float
### getArea() {#getArea--}
```
public Area getArea()
```


Obtient le [getArea()](../../com.aspose.cells/chartpoint\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Obtient le [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getBorderWidthPx() {#getBorderWidthPx--}
```
public int getBorderWidthPx()
```


Obtient la largeur de la bordure en pixels après l'appel de la méthode Chart.Calculate().

**Returns:**
int
### getBottomPointCount() {#getBottomPointCount--}
```
public int getBottomPointCount()
```


Obtient le nombre de points inférieurs après l'appel de la méthode Chart.Calculate().

**Returns:**
int
### getBottomPointXPx(int index) {#getBottomPointXPx-int-}
```
public float getBottomPointXPx(int index)
```


Obtient la coordonnée x du point inférieur de la forme après l'appel de la méthode Chart.Calculate(). S'applique aux graphiques 3D : Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
float
### getBottomPointYPx(int index) {#getBottomPointYPx-int-}
```
public float getBottomPointYPx(int index)
```


Obtient la coordonnée y du point inférieur de la forme après l'appel de la méthode Chart.Calculate(). S'applique aux graphiques 3D : Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
float
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Renvoie un objet [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) qui représente l'étiquette de données associée à ce point de graphique.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDoughnutInnerRadius() {#getDoughnutInnerRadius--}
```
public int getDoughnutInnerRadius()
```


Obtient le rayon interne de la tranche du Donut en pixels après l'appel de la méthode Chart.Calculate(). S'applique au graphique Doughnut.

**Returns:**
int
### getEndAngle() {#getEndAngle--}
```
public float getEndAngle()
```


Obtient l'angle final de la section du camembert, mesuré en degrés dans le sens horaire à partir de l'axe x après l'appel de la méthode Chart.Calculate(). S'applique au graphique Pie.

**Returns:**
float
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


La distance d'une tranche de diagramme circulaire ouverte du centre du diagramme circulaire est exprimée en pourcentage du diamètre du diagramme.

**Returns:**
int
### getInnerArcEndPointXPx() {#getInnerArcEndPointXPx--}
```
public float getInnerArcEndPointXPx()
```


Obtient la coordonnée x du point final de la section du camembert après l'appel de la méthode Chart.Calculate(). S'applique aux graphiques Doughnut.

**Returns:**
float
### getInnerArcEndPointYPx() {#getInnerArcEndPointYPx--}
```
public float getInnerArcEndPointYPx()
```


Obtient la coordonnée y du point final de la section du camembert après l'appel de la méthode Chart.Calculate(). S'applique au graphique Doughnut.

**Returns:**
float
### getInnerArcStartPointXPx() {#getInnerArcStartPointXPx--}
```
public float getInnerArcStartPointXPx()
```


Obtient la coordonnée x du point de départ de la section du camembert après l'appel de la méthode Chart.Calculate(). S'applique au graphique Doughnut.

**Returns:**
float
### getInnerArcStartPointYPx() {#getInnerArcStartPointYPx--}
```
public float getInnerArcStartPointYPx()
```


Obtient la coordonnée y du point de départ de la section du diagramme circulaire après l’appel de la méthode Chart.Calculate(). S’applique au diagramme en anneau.

**Returns:**
float
### getInnerRadiusPx() {#getInnerRadiusPx--}
```
public int getInnerRadiusPx()
```


Obtient le rayon interne de la tranche du diagramme en anneau en unités de pixels après l’appel de la méthode Chart.Calculate(). S’applique au diagramme en anneau.

**Remarks**

REMARQUE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété ChartPoint.DoughnutInnerRadius. Cette propriété sera supprimée 12 mois plus tard à compter de juin 2024. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
int
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


Obtient le [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getOnCategoryAxisPointCount() {#getOnCategoryAxisPointCount--}
```
public int getOnCategoryAxisPointCount()
```


Obtient le nombre de points sur l’axe des catégories après l’appel de la méthode Chart.Calculate(). S’applique uniquement aux graphiques en aires.

**Remarks**

Le graphique en aires 2D renvoie 1, le graphique en aires 3D renvoie 2.

**Returns:**
int
### getOnCategoryAxisPointXPx(int index) {#getOnCategoryAxisPointXPx-int-}
```
public float getOnCategoryAxisPointXPx(int index)
```


Obtient la coordonnée x du point sur l’axe des catégories après l’appel de la méthode Chart.Calculate(). S’applique uniquement au graphique en aires.

**Remarks**

Graphique en aires 2D : l’indice est 0. Graphique en aires 3D : l’indice est 0 ou 1.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
float
### getOnCategoryAxisPointYPx(int index) {#getOnCategoryAxisPointYPx-int-}
```
public float getOnCategoryAxisPointYPx(int index)
```


Obtient la coordonnée y du point sur l’axe des catégories après l’appel de la méthode Chart.Calculate(). S’applique uniquement au graphique en aires.

**Remarks**

Graphique en aires 2D : l’indice est 0. Graphique en aires 3D : l’indice est 0 ou 1.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
float
### getRadiusPx() {#getRadiusPx--}
```
public int getRadiusPx()
```


Obtient le rayon de la bulle, du diagramme circulaire ou du beignet en pixels après l'appel de la méthode Chart.Calculate().

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Vrai si le point de graphique possède une ombre.

**Returns:**
boolean
### getShapeHeight() {#getShapeHeight--}
```
public int getShapeHeight()
```


Obtient la hauteur en unités de 1/4000 de la hauteur du graphique après l'appel de la méthode Chart.Calculate().

**Returns:**
int
### getShapeHeightPx() {#getShapeHeightPx--}
```
public int getShapeHeightPx()
```


Obtient la hauteur en pixels après l'appel de la méthode Chart.Calculate().

**Returns:**
int
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Obtient l'objet [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) qui contient les propriétés visuelles de forme du ChartPoint.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShapeWidth() {#getShapeWidth--}
```
public int getShapeWidth()
```


Obtient la largeur en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate().

**Returns:**
int
### getShapeWidthPx() {#getShapeWidthPx--}
```
public int getShapeWidthPx()
```


Obtient la largeur en pixels après l'appel de la méthode Chart.Calculate().

**Returns:**
int
### getShapeX() {#getShapeX--}
```
public int getShapeX()
```


Obtient la coordonnée x du coin supérieur gauche en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate().

**Returns:**
int
### getShapeXPx() {#getShapeXPx--}
```
public int getShapeXPx()
```


Obtient la coordonnée x du coin supérieur gauche en pixels après l'appel de la méthode Chart.Calculate().

**Returns:**
int
### getShapeY() {#getShapeY--}
```
public int getShapeY()
```


Obtient la coordonnée y du coin supérieur gauche en unités de 1/4000 de la hauteur du graphique après l'appel de la méthode Chart.Calculate().

**Returns:**
int
### getShapeYPx() {#getShapeYPx--}
```
public int getShapeYPx()
```


Obtient la coordonnée y du coin supérieur gauche en pixels après l'appel de la méthode Chart.Calculate().

**Returns:**
int
### getStartAngle() {#getStartAngle--}
```
public float getStartAngle()
```


Obtient l’angle de départ de la section du diagramme circulaire, mesuré en degrés dans le sens des aiguilles d’une montre à partir de l’axe x après l’appel de la méthode Chart.Calculate(). S’applique au diagramme circulaire.

**Returns:**
float
### getTopPointCount() {#getTopPointCount--}
```
public int getTopPointCount()
```


Obtient le nombre de points supérieurs après l'appel de la méthode Chart.Calculate().

**Returns:**
int
### getTopPointXPx(int index) {#getTopPointXPx-int-}
```
public float getTopPointXPx(int index)
```


Obtient la coordonnée x du point supérieur de la forme après l’appel de la méthode Chart.Calculate(). S’applique aux graphiques 3D : Column3D, Bar3D, Cone, Cylinder, Pyramid et Area3D

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
float
### getTopPointYPx(int index) {#getTopPointYPx-int-}
```
public float getTopPointYPx(int index)
```


Obtient la coordonnée y du point supérieur de la forme après l’appel de la méthode Chart.Calculate(). S’applique aux graphiques 3D : Column3D, Bar3D, Cone, Cylinder, Pyramid et Area3D.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
float
### getXValue() {#getXValue--}
```
public Object getXValue()
```


Obtient la valeur X du point du graphique.

**Returns:**
java.lang.Object
### getXValueType() {#getXValueType--}
```
public int getXValueType()
```


Obtient le type de valeur X du point du graphique.

Voir [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getYValue() {#getYValue--}
```
public Object getYValue()
```


Obtient la valeur Y du point du graphique.

**Returns:**
java.lang.Object
### getYValueType() {#getYValueType--}
```
public int getYValueType()
```


Obtient le type de valeur Y du point du graphique.

Voir [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isInSecondaryPlot() {#isInSecondaryPlot--}
```
public boolean isInSecondaryPlot()
```


Obtient une valeur indiquant si ce point de données se trouve dans le deuxième camembert ou barre d'un graphique en camembert de camembert ou barre de camembert.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```


La distance d'une tranche de diagramme circulaire ouverte du centre du diagramme circulaire est exprimée en pourcentage du diamètre du diagramme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setInSecondaryPlot(boolean value) {#setInSecondaryPlot-boolean-}
```
public void setInSecondaryPlot(boolean value)
```


Définit une valeur indiquant si ce point de données se trouve dans le deuxième camembert ou barre d'un graphique en camembert de camembert ou barre de camembert.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Vrai si le point de graphique possède une ombre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setXValue(Object value) {#setXValue-java.lang.Object-}
```
public void setXValue(Object value)
```


Définit la valeur X du point du graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

### setYValue(Object value) {#setYValue-java.lang.Object-}
```
public void setYValue(Object value)
```


Définit la valeur Y du point du graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

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

