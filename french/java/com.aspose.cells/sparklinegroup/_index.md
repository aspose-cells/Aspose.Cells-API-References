---
title: "SparklineGroup"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "est organisé en groupe de sparkline."
type: docs
url: /fr/java/com.aspose.cells/sparklinegroup/
---

**Inheritance:**
java.lang.Object
```
public class SparklineGroup
```

[Sparkline](../../com.aspose.cells/sparkline) is organized into a sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, "A1:D1", false, ca);
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         // Create CellsColor
         CellsColor clr = book.createCellsColor();
         clr.setColor(Color.getOrange());
         group.setSeriesColor(clr);
 
         // set the high points are colored green and the low points are colored red
         group.setShowHighPoint(true);
         group.setShowLowPoint(true);
         group.getHighPointColor().setColor(Color.getGreen());
         group.getLowPointColor().setColor(Color.getRed());
         // set line weight 
         group.setLineWeight(1.0);
         book.save("output.xlsx", SaveFormat.XLSX);
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDisplayHidden()](#getDisplayHidden--) | Indique s'il faut afficher les données dans les lignes et colonnes masquées. |
| [getFirstPointColor()](#getFirstPointColor--) | Obtient la couleur du premier point de données dans le groupe de sparkline. |
| [getHighPointColor()](#getHighPointColor--) | Obtient la couleur des points les plus élevés de données dans le groupe de sparkline. |
| [getHorizontalAxisColor()](#getHorizontalAxisColor--) | Obtient la couleur de l'axe horizontal dans le groupe de sparkline. |
| [getHorizontalAxisDateRange()](#getHorizontalAxisDateRange--) | Représente la plage qui contient les valeurs de date pour les données de sparkline. |
| [getLastPointColor()](#getLastPointColor--) | Obtient la couleur du dernier point de données dans le groupe de sparkline. |
| [getLineWeight()](#getLineWeight--) | Obtient l'épaisseur de ligne de chaque sparkline linéaire dans le groupe de sparkline, en points. |
| [getLowPointColor()](#getLowPointColor--) | Obtient la couleur des points les plus bas de données dans le groupe de sparkline. |
| [getMarkersColor()](#getMarkersColor--) | Obtient la couleur des points de chaque sparkline linéaire dans le groupe de sparkline. |
| [getNegativePointsColor()](#getNegativePointsColor--) | Obtient la couleur des valeurs négatives du groupe de sparkline. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Indique comment tracer les cellules vides. |
| [getPlotRightToLeft()](#getPlotRightToLeft--) | Indique si les données du tracé sont de droite à gauche. |
| [getPresetStyle()](#getPresetStyle--) | Obtient le type de style prédéfini du groupe de sparkline. |
| [getSeriesColor()](#getSeriesColor--) | Obtient la couleur des sparklines dans le groupe de sparkline. |
| [getShowFirstPoint()](#getShowFirstPoint--) | Indique s'il faut mettre en évidence le premier point de données dans le groupe de sparkline. |
| [getShowHighPoint()](#getShowHighPoint--) | Indique si les points les plus élevés des données du groupe de sparkline doivent être mis en évidence. |
| [getShowHorizontalAxis()](#getShowHorizontalAxis--) | Indique si l'axe horizontal du sparkline doit être affiché. |
| [getShowLastPoint()](#getShowLastPoint--) | Indique si le dernier point de données du groupe de sparkline doit être mis en évidence. |
| [getShowLowPoint()](#getShowLowPoint--) | Indique si les points les plus bas des données du groupe de sparkline doivent être mis en évidence. |
| [getShowMarkers()](#getShowMarkers--) | Indique si chaque point de chaque sparkline en ligne du groupe de sparkline doit être mis en évidence. |
| [getShowNegativePoints()](#getShowNegativePoints--) | Indique si les valeurs négatives du groupe de sparkline doivent être mises en évidence avec une couleur ou un marqueur différent. |
| [getSparklineCollection()](#getSparklineCollection--) | Obtient la collection d'objets [Sparkline](../../com.aspose.cells/sparkline). |
| [getSparklines()](#getSparklines--) | Obtient la collection d'objets [Sparkline](../../com.aspose.cells/sparkline). |
| [getType()](#getType--) | Indique le type de sparkline du groupe de sparkline. |
| [getVerticalAxisMaxValue()](#getVerticalAxisMaxValue--) | Obtient la valeur maximale personnalisée pour l'axe vertical. |
| [getVerticalAxisMaxValueType()](#getVerticalAxisMaxValueType--) | Représente le type de valeur maximale de l'axe vertical. |
| [getVerticalAxisMinValue()](#getVerticalAxisMinValue--) | Obtient la valeur minimale personnalisée pour l'axe vertical. |
| [getVerticalAxisMinValueType()](#getVerticalAxisMinValueType--) | Représente le type de valeur minimale de l'axe vertical. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [resetRanges(String dataRange, boolean isVertical, CellArea locationRange)](#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-) | Réinitialise la plage de données et la plage d'emplacement du groupe de sparkline. |
| [setDisplayHidden(boolean value)](#setDisplayHidden-boolean-) | Indique s'il faut afficher les données dans les lignes et colonnes masquées. |
| [setFirstPointColor(CellsColor value)](#setFirstPointColor-com.aspose.cells.CellsColor-) | Définit la couleur du premier point de données du groupe de sparkline. |
| [setHighPointColor(CellsColor value)](#setHighPointColor-com.aspose.cells.CellsColor-) | Définit la couleur des points les plus élevés des données du groupe de sparkline. |
| [setHorizontalAxisColor(CellsColor value)](#setHorizontalAxisColor-com.aspose.cells.CellsColor-) | Définit la couleur de l'axe horizontal du groupe de sparkline. |
| [setHorizontalAxisDateRange(String value)](#setHorizontalAxisDateRange-java.lang.String-) | Représente la plage qui contient les valeurs de date pour les données de sparkline. |
| [setLastPointColor(CellsColor value)](#setLastPointColor-com.aspose.cells.CellsColor-) | Définit la couleur du dernier point de données du groupe de sparkline. |
| [setLineWeight(double value)](#setLineWeight-double-) | Définit l'épaisseur de la ligne dans chaque sparkline en ligne du groupe de sparkline, en points. |
| [setLowPointColor(CellsColor value)](#setLowPointColor-com.aspose.cells.CellsColor-) | Définit la couleur des points les plus bas des données du groupe de sparkline. |
| [setMarkersColor(CellsColor value)](#setMarkersColor-com.aspose.cells.CellsColor-) | Définit la couleur des points dans chaque sparkline en ligne du groupe de sparkline. |
| [setNegativePointsColor(CellsColor value)](#setNegativePointsColor-com.aspose.cells.CellsColor-) | Définit la couleur des valeurs négatives du groupe de sparkline. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | Indique comment tracer les cellules vides. |
| [setPlotRightToLeft(boolean value)](#setPlotRightToLeft-boolean-) | Indique si les données du tracé sont de droite à gauche. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | Définit le type de style prédéfini du groupe de sparkline. |
| [setSeriesColor(CellsColor value)](#setSeriesColor-com.aspose.cells.CellsColor-) | Définit la couleur des sparklines du groupe de sparkline. |
| [setShowFirstPoint(boolean value)](#setShowFirstPoint-boolean-) | Indique s'il faut mettre en évidence le premier point de données dans le groupe de sparkline. |
| [setShowHighPoint(boolean value)](#setShowHighPoint-boolean-) | Indique si les points les plus élevés des données du groupe de sparkline doivent être mis en évidence. |
| [setShowHorizontalAxis(boolean value)](#setShowHorizontalAxis-boolean-) | Indique si l'axe horizontal du sparkline doit être affiché. |
| [setShowLastPoint(boolean value)](#setShowLastPoint-boolean-) | Indique si le dernier point de données du groupe de sparkline doit être mis en évidence. |
| [setShowLowPoint(boolean value)](#setShowLowPoint-boolean-) | Indique si les points les plus bas des données du groupe de sparkline doivent être mis en évidence. |
| [setShowMarkers(boolean value)](#setShowMarkers-boolean-) | Indique si chaque point de chaque sparkline en ligne du groupe de sparkline doit être mis en évidence. |
| [setShowNegativePoints(boolean value)](#setShowNegativePoints-boolean-) | Indique si les valeurs négatives du groupe de sparkline doivent être mises en évidence avec une couleur ou un marqueur différent. |
| [setType(int value)](#setType-int-) | Indique le type de sparkline du groupe de sparkline. |
| [setVerticalAxisMaxValue(double value)](#setVerticalAxisMaxValue-double-) | Définit la valeur maximale personnalisée pour l'axe vertical. |
| [setVerticalAxisMaxValue(int type, double value)](#setVerticalAxisMaxValue-int-double-) | Définit la valeur maximale personnalisée pour l'axe vertical du sparkline avec le type de valeur d'axe spécifié. |
| [setVerticalAxisMaxValueType(int value)](#setVerticalAxisMaxValueType-int-) | Représente le type de valeur maximale de l'axe vertical. |
| [setVerticalAxisMinValue(double value)](#setVerticalAxisMinValue-double-) | Définit la valeur minimale personnalisée pour l'axe vertical. |
| [setVerticalAxisMinValue(int type, double value)](#setVerticalAxisMinValue-int-double-) | Définit la valeur minimale personnalisée pour l'axe vertical du sparkline avec le type de valeur d'axe spécifié. |
| [setVerticalAxisMinValueType(int value)](#setVerticalAxisMinValueType-int-) | Représente le type de valeur minimale de l'axe vertical. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDisplayHidden() {#getDisplayHidden--}
```
public boolean getDisplayHidden()
```


Indique s'il faut afficher les données dans les lignes et colonnes masquées.

**Returns:**
boolean
### getFirstPointColor() {#getFirstPointColor--}
```
public CellsColor getFirstPointColor()
```


Obtient la couleur du premier point de données dans le groupe de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHighPointColor() {#getHighPointColor--}
```
public CellsColor getHighPointColor()
```


Obtient la couleur des points les plus élevés de données dans le groupe de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisColor() {#getHorizontalAxisColor--}
```
public CellsColor getHorizontalAxisColor()
```


Obtient la couleur de l'axe horizontal dans le groupe de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisDateRange() {#getHorizontalAxisDateRange--}
```
public String getHorizontalAxisDateRange()
```


Représente la plage qui contient les valeurs de date pour les données de sparkline.

**Returns:**
java.lang.String
### getLastPointColor() {#getLastPointColor--}
```
public CellsColor getLastPointColor()
```


Obtient la couleur du dernier point de données dans le groupe de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getLineWeight() {#getLineWeight--}
```
public double getLineWeight()
```


Obtient l'épaisseur de ligne de chaque sparkline linéaire dans le groupe de sparkline, en points.

**Returns:**
double
### getLowPointColor() {#getLowPointColor--}
```
public CellsColor getLowPointColor()
```


Obtient la couleur des points les plus bas de données dans le groupe de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getMarkersColor() {#getMarkersColor--}
```
public CellsColor getMarkersColor()
```


Obtient la couleur des points de chaque sparkline linéaire dans le groupe de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getNegativePointsColor() {#getNegativePointsColor--}
```
public CellsColor getNegativePointsColor()
```


Obtient la couleur des valeurs négatives du groupe de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


Indique comment tracer les cellules vides.

Voir [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotRightToLeft() {#getPlotRightToLeft--}
```
public boolean getPlotRightToLeft()
```


Indique si les données du tracé sont de droite à gauche.

**Returns:**
boolean
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


Obtient le type de style prédéfini du groupe de sparkline.

Voir [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

Si cette propriété est définie, ces propriétés : SeriesColor, NegativePointsColor, HorizontalAxisColor, MarkersColor, FirstPointColor, LastPointColor, HighPointColor, LowPointColor seront couvertes. Veuillez donc définir d'abord la propriété, puis les autres.

**Returns:**
int
### getSeriesColor() {#getSeriesColor--}
```
public CellsColor getSeriesColor()
```


Obtient la couleur des sparklines dans le groupe de sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getShowFirstPoint() {#getShowFirstPoint--}
```
public boolean getShowFirstPoint()
```


Indique s'il faut mettre en évidence le premier point de données dans le groupe de sparkline.

**Returns:**
boolean
### getShowHighPoint() {#getShowHighPoint--}
```
public boolean getShowHighPoint()
```


Indique si les points les plus élevés des données du groupe de sparkline doivent être mis en évidence.

**Returns:**
boolean
### getShowHorizontalAxis() {#getShowHorizontalAxis--}
```
public boolean getShowHorizontalAxis()
```


Indique s'il faut afficher l'axe horizontal du sparkline. L'axe horizontal apparaît si le sparkline possède des données qui traversent l'axe zéro.

**Returns:**
boolean
### getShowLastPoint() {#getShowLastPoint--}
```
public boolean getShowLastPoint()
```


Indique si le dernier point de données du groupe de sparkline doit être mis en évidence.

**Returns:**
boolean
### getShowLowPoint() {#getShowLowPoint--}
```
public boolean getShowLowPoint()
```


Indique si les points les plus bas des données du groupe de sparkline doivent être mis en évidence.

**Returns:**
boolean
### getShowMarkers() {#getShowMarkers--}
```
public boolean getShowMarkers()
```


Indique si chaque point de chaque sparkline en ligne du groupe de sparkline doit être mis en évidence.

**Returns:**
boolean
### getShowNegativePoints() {#getShowNegativePoints--}
```
public boolean getShowNegativePoints()
```


Indique si les valeurs négatives du groupe de sparkline doivent être mises en évidence avec une couleur ou un marqueur différent.

**Returns:**
boolean
### getSparklineCollection() {#getSparklineCollection--}
```
public SparklineCollection getSparklineCollection()
```


Obtient la collection d'objets [Sparkline](../../com.aspose.cells/sparkline).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété SparklineGroup.Sparklines. Cette propriété sera supprimée 12 mois plus tard, à compter de novembre 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getSparklines() {#getSparklines--}
```
public SparklineCollection getSparklines()
```


Obtient la collection d'objets [Sparkline](../../com.aspose.cells/sparkline).

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getType() {#getType--}
```
public int getType()
```


Indique le type de sparkline du groupe de sparkline.

Voir [SparklineType](../../com.aspose.cells/sparklinetype).

**Returns:**
int
### getVerticalAxisMaxValue() {#getVerticalAxisMaxValue--}
```
public double getVerticalAxisMaxValue()
```


Obtient la valeur maximale personnalisée pour l'axe vertical.

**Remarks**

Si cette propriété est définie, [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) sera [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Returns:**
double
### getVerticalAxisMaxValueType() {#getVerticalAxisMaxValueType--}
```
public int getVerticalAxisMaxValueType()
```


Représente le type de valeur maximale de l'axe vertical.

Voir [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Returns:**
int
### getVerticalAxisMinValue() {#getVerticalAxisMinValue--}
```
public double getVerticalAxisMinValue()
```


Obtient la valeur minimale personnalisée pour l'axe vertical.

**Remarks**

Si cette propriété est définie, [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) sera [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Returns:**
double
### getVerticalAxisMinValueType() {#getVerticalAxisMinValueType--}
```
public int getVerticalAxisMinValueType()
```


Représente le type de valeur minimale de l'axe vertical.

Voir [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### resetRanges(String dataRange, boolean isVertical, CellArea locationRange) {#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-}
```
public void resetRanges(String dataRange, boolean isVertical, CellArea locationRange)
```


Réinitialise la plage de données et la plage d'emplacement du groupe de sparkline. Cette méthode effacera les éléments sparkline d'origine du groupe et créera de nouveaux éléments sparkline pour les nouvelles plages.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dataRange | java.lang.String | Spécifie la nouvelle plage de données du groupe de sparkline. |
| isVertical | boolean | Spécifie s'il faut tracer les sparklines à partir de la nouvelle plage de données par ligne ou par colonne. |
| locationRange | [CellArea](../../com.aspose.cells/cellarea) | Spécifie où placer les sparklines. |

### setDisplayHidden(boolean value) {#setDisplayHidden-boolean-}
```
public void setDisplayHidden(boolean value)
```


Indique s'il faut afficher les données dans les lignes et colonnes masquées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFirstPointColor(CellsColor value) {#setFirstPointColor-com.aspose.cells.CellsColor-}
```
public void setFirstPointColor(CellsColor value)
```


Définit la couleur du premier point de données du groupe de sparkline.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHighPointColor(CellsColor value) {#setHighPointColor-com.aspose.cells.CellsColor-}
```
public void setHighPointColor(CellsColor value)
```


Définit la couleur des points les plus élevés des données du groupe de sparkline.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisColor(CellsColor value) {#setHorizontalAxisColor-com.aspose.cells.CellsColor-}
```
public void setHorizontalAxisColor(CellsColor value)
```


Définit la couleur de l'axe horizontal du groupe de sparkline.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisDateRange(String value) {#setHorizontalAxisDateRange-java.lang.String-}
```
public void setHorizontalAxisDateRange(String value)
```


Représente la plage qui contient les valeurs de date pour les données de sparkline.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setLastPointColor(CellsColor value) {#setLastPointColor-com.aspose.cells.CellsColor-}
```
public void setLastPointColor(CellsColor value)
```


Définit la couleur du dernier point de données du groupe de sparkline.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setLineWeight(double value) {#setLineWeight-double-}
```
public void setLineWeight(double value)
```


Définit l'épaisseur de la ligne dans chaque sparkline en ligne du groupe de sparkline, en points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setLowPointColor(CellsColor value) {#setLowPointColor-com.aspose.cells.CellsColor-}
```
public void setLowPointColor(CellsColor value)
```


Définit la couleur des points les plus bas des données du groupe de sparkline.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setMarkersColor(CellsColor value) {#setMarkersColor-com.aspose.cells.CellsColor-}
```
public void setMarkersColor(CellsColor value)
```


Définit la couleur des points dans chaque sparkline en ligne du groupe de sparkline.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setNegativePointsColor(CellsColor value) {#setNegativePointsColor-com.aspose.cells.CellsColor-}
```
public void setNegativePointsColor(CellsColor value)
```


Définit la couleur des valeurs négatives du groupe de sparkline.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


Indique comment tracer les cellules vides.

Voir [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPlotRightToLeft(boolean value) {#setPlotRightToLeft-boolean-}
```
public void setPlotRightToLeft(boolean value)
```


Indique si les données du tracé sont de droite à gauche.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


Définit le type de style prédéfini du groupe de sparkline.

Voir [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

Si cette propriété est définie, ces propriétés : SeriesColor, NegativePointsColor, HorizontalAxisColor, MarkersColor, FirstPointColor, LastPointColor, HighPointColor, LowPointColor seront couvertes. Veuillez donc définir d'abord la propriété, puis les autres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSeriesColor(CellsColor value) {#setSeriesColor-com.aspose.cells.CellsColor-}
```
public void setSeriesColor(CellsColor value)
```


Définit la couleur des sparklines du groupe de sparkline.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setShowFirstPoint(boolean value) {#setShowFirstPoint-boolean-}
```
public void setShowFirstPoint(boolean value)
```


Indique s'il faut mettre en évidence le premier point de données dans le groupe de sparkline.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowHighPoint(boolean value) {#setShowHighPoint-boolean-}
```
public void setShowHighPoint(boolean value)
```


Indique si les points les plus élevés des données du groupe de sparkline doivent être mis en évidence.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowHorizontalAxis(boolean value) {#setShowHorizontalAxis-boolean-}
```
public void setShowHorizontalAxis(boolean value)
```


Indique s'il faut afficher l'axe horizontal du sparkline. L'axe horizontal apparaît si le sparkline possède des données qui traversent l'axe zéro.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowLastPoint(boolean value) {#setShowLastPoint-boolean-}
```
public void setShowLastPoint(boolean value)
```


Indique si le dernier point de données du groupe de sparkline doit être mis en évidence.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowLowPoint(boolean value) {#setShowLowPoint-boolean-}
```
public void setShowLowPoint(boolean value)
```


Indique si les points les plus bas des données du groupe de sparkline doivent être mis en évidence.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowMarkers(boolean value) {#setShowMarkers-boolean-}
```
public void setShowMarkers(boolean value)
```


Indique si chaque point de chaque sparkline en ligne du groupe de sparkline doit être mis en évidence.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowNegativePoints(boolean value) {#setShowNegativePoints-boolean-}
```
public void setShowNegativePoints(boolean value)
```


Indique si les valeurs négatives du groupe de sparkline doivent être mises en évidence avec une couleur ou un marqueur différent.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Indique le type de sparkline du groupe de sparkline.

Voir [SparklineType](../../com.aspose.cells/sparklinetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setVerticalAxisMaxValue(double value) {#setVerticalAxisMaxValue-double-}
```
public void setVerticalAxisMaxValue(double value)
```


Définit la valeur maximale personnalisée pour l'axe vertical.

**Remarks**

Si cette propriété est définie, [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) sera [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setVerticalAxisMaxValue(int type, double value) {#setVerticalAxisMaxValue-int-double-}
```
public void setVerticalAxisMaxValue(int type, double value)
```


Définit la valeur maximale personnalisée pour l'axe vertical du sparkline avec le type de valeur d'axe spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). Type qui spécifie comment la valeur maximale de l'axe est appliquée. |
| value | double | Valeur maximale personnalisée de l'axe vertical. Ignorée si le type n'est pas [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM) |

### setVerticalAxisMaxValueType(int value) {#setVerticalAxisMaxValueType-int-}
```
public void setVerticalAxisMaxValueType(int value)
```


Représente le type de valeur maximale de l'axe vertical.

Voir [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setVerticalAxisMinValue(double value) {#setVerticalAxisMinValue-double-}
```
public void setVerticalAxisMinValue(double value)
```


Définit la valeur minimale personnalisée pour l'axe vertical.

**Remarks**

Si cette propriété est définie, [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) sera [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setVerticalAxisMinValue(int type, double value) {#setVerticalAxisMinValue-int-double-}
```
public void setVerticalAxisMinValue(int type, double value)
```


Définit la valeur minimale personnalisée pour l'axe vertical du sparkline avec le type de valeur d'axe spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). Type qui spécifie comment la valeur minimale de l'axe est appliquée. |
| value | double | Valeur minimale personnalisée de l'axe vertical. Ignorée si le type n'est pas [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM) |

### setVerticalAxisMinValueType(int value) {#setVerticalAxisMinValueType-int-}
```
public void setVerticalAxisMinValueType(int value)
```


Représente le type de valeur minimale de l'axe vertical.

Voir [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

