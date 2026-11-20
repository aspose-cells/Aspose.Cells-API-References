---
title: "SparklineGroup"
second_title: "Справочник API Aspose.Cells for Java"
description: "организовано в группу спарклайнов."
type: docs
url: /ru/java/com.aspose.cells/sparklinegroup/
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
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDisplayHidden()](#getDisplayHidden--) | Указывает, показывать ли данные в скрытых строках и столбцах. |
| [getFirstPointColor()](#getFirstPointColor--) | Получает цвет первой точки данных в группе спарклайнов. |
| [getHighPointColor()](#getHighPointColor--) | Получает цвет самых высоких точек данных в группе спарклайнов. |
| [getHorizontalAxisColor()](#getHorizontalAxisColor--) | Получает цвет горизонтальной оси в группе спарклайнов. |
| [getHorizontalAxisDateRange()](#getHorizontalAxisDateRange--) | Представляет диапазон, содержащий значения дат для данных спарклайна. |
| [getLastPointColor()](#getLastPointColor--) | Получает цвет последней точки данных в группе спарклайнов. |
| [getLineWeight()](#getLineWeight--) | Получает толщину линии в каждом линейном спарклайне в группе спарклайнов, в единицах пунктов. |
| [getLowPointColor()](#getLowPointColor--) | Получает цвет самых низких точек данных в группе спарклайнов. |
| [getMarkersColor()](#getMarkersColor--) | Получает цвет точек в каждом линейном спарклайне в группе спарклайнов. |
| [getNegativePointsColor()](#getNegativePointsColor--) | Получает цвет отрицательных значений в группе спарклайнов. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Указывает, как отображать пустые ячейки. |
| [getPlotRightToLeft()](#getPlotRightToLeft--) | Указывает, отображаются ли данные справа налево. |
| [getPresetStyle()](#getPresetStyle--) | Получает тип предустановленного стиля группы спарклайнов. |
| [getSeriesColor()](#getSeriesColor--) | Получает цвет спарклайнов в группе спарклайнов. |
| [getShowFirstPoint()](#getShowFirstPoint--) | Указывает, выделять ли первую точку данных в группе спарклайнов. |
| [getShowHighPoint()](#getShowHighPoint--) | Указывает, следует ли выделять наивысшие точки данных в группе спарклайнов. |
| [getShowHorizontalAxis()](#getShowHorizontalAxis--) | Указывает, следует ли отображать горизонтальную ось спарклайна. |
| [getShowLastPoint()](#getShowLastPoint--) | Указывает, следует ли выделять последнюю точку данных в группе спарклайнов. |
| [getShowLowPoint()](#getShowLowPoint--) | Указывает, следует ли выделять наименьшие точки данных в группе спарклайнов. |
| [getShowMarkers()](#getShowMarkers--) | Указывает, следует ли выделять каждую точку в каждом линейном спарклайне в группе спарклайнов. |
| [getShowNegativePoints()](#getShowNegativePoints--) | Указывает, следует ли выделять отрицательные значения в группе спарклайнов другим цветом или маркером. |
| [getSparklineCollection()](#getSparklineCollection--) | Получает коллекцию объектов [Sparkline](../../com.aspose.cells/sparkline). |
| [getSparklines()](#getSparklines--) | Получает коллекцию объектов [Sparkline](../../com.aspose.cells/sparkline). |
| [getType()](#getType--) | Указывает тип спарклайна в группе спарклайнов. |
| [getVerticalAxisMaxValue()](#getVerticalAxisMaxValue--) | Получает пользовательское максимальное значение для вертикальной оси. |
| [getVerticalAxisMaxValueType()](#getVerticalAxisMaxValueType--) | Представляет тип максимального значения вертикальной оси. |
| [getVerticalAxisMinValue()](#getVerticalAxisMinValue--) | Получает пользовательское минимальное значение для вертикальной оси. |
| [getVerticalAxisMinValueType()](#getVerticalAxisMinValueType--) | Представляет тип минимального значения вертикальной оси. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [resetRanges(String dataRange, boolean isVertical, CellArea locationRange)](#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-) | Сбрасывает диапазон данных и диапазон расположения группы спарклайнов. |
| [setDisplayHidden(boolean value)](#setDisplayHidden-boolean-) | Указывает, показывать ли данные в скрытых строках и столбцах. |
| [setFirstPointColor(CellsColor value)](#setFirstPointColor-com.aspose.cells.CellsColor-) | Устанавливает цвет первой точки данных в группе спарклайнов. |
| [setHighPointColor(CellsColor value)](#setHighPointColor-com.aspose.cells.CellsColor-) | Устанавливает цвет наивысших точек данных в группе спарклайнов. |
| [setHorizontalAxisColor(CellsColor value)](#setHorizontalAxisColor-com.aspose.cells.CellsColor-) | Устанавливает цвет горизонтальной оси в группе спарклайнов. |
| [setHorizontalAxisDateRange(String value)](#setHorizontalAxisDateRange-java.lang.String-) | Представляет диапазон, содержащий значения дат для данных спарклайна. |
| [setLastPointColor(CellsColor value)](#setLastPointColor-com.aspose.cells.CellsColor-) | Устанавливает цвет последней точки данных в группе спарклайнов. |
| [setLineWeight(double value)](#setLineWeight-double-) | Устанавливает толщину линии в каждом линейном спарклайне в группе спарклайнов, в единицах точек. |
| [setLowPointColor(CellsColor value)](#setLowPointColor-com.aspose.cells.CellsColor-) | Устанавливает цвет наименьших точек данных в группе спарклайнов. |
| [setMarkersColor(CellsColor value)](#setMarkersColor-com.aspose.cells.CellsColor-) | Устанавливает цвет точек в каждом линейном спарклайне в группе спарклайнов. |
| [setNegativePointsColor(CellsColor value)](#setNegativePointsColor-com.aspose.cells.CellsColor-) | Устанавливает цвет отрицательных значений в группе спарклайнов. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | Указывает, как отображать пустые ячейки. |
| [setPlotRightToLeft(boolean value)](#setPlotRightToLeft-boolean-) | Указывает, отображаются ли данные справа налево. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | Устанавливает тип предустановленного стиля группы спарклайнов. |
| [setSeriesColor(CellsColor value)](#setSeriesColor-com.aspose.cells.CellsColor-) | Устанавливает цвет спарклайнов в группе спарклайнов. |
| [setShowFirstPoint(boolean value)](#setShowFirstPoint-boolean-) | Указывает, выделять ли первую точку данных в группе спарклайнов. |
| [setShowHighPoint(boolean value)](#setShowHighPoint-boolean-) | Указывает, следует ли выделять наивысшие точки данных в группе спарклайнов. |
| [setShowHorizontalAxis(boolean value)](#setShowHorizontalAxis-boolean-) | Указывает, следует ли отображать горизонтальную ось спарклайна. |
| [setShowLastPoint(boolean value)](#setShowLastPoint-boolean-) | Указывает, следует ли выделять последнюю точку данных в группе спарклайнов. |
| [setShowLowPoint(boolean value)](#setShowLowPoint-boolean-) | Указывает, следует ли выделять наименьшие точки данных в группе спарклайнов. |
| [setShowMarkers(boolean value)](#setShowMarkers-boolean-) | Указывает, следует ли выделять каждую точку в каждом линейном спарклайне в группе спарклайнов. |
| [setShowNegativePoints(boolean value)](#setShowNegativePoints-boolean-) | Указывает, следует ли выделять отрицательные значения в группе спарклайнов другим цветом или маркером. |
| [setType(int value)](#setType-int-) | Указывает тип спарклайна в группе спарклайнов. |
| [setVerticalAxisMaxValue(double value)](#setVerticalAxisMaxValue-double-) | Устанавливает пользовательское максимальное значение для вертикальной оси. |
| [setVerticalAxisMaxValue(int type, double value)](#setVerticalAxisMaxValue-int-double-) | Устанавливает пользовательское максимальное значение для вертикальной оси спарклайна с указанным типом значения оси. |
| [setVerticalAxisMaxValueType(int value)](#setVerticalAxisMaxValueType-int-) | Представляет тип максимального значения вертикальной оси. |
| [setVerticalAxisMinValue(double value)](#setVerticalAxisMinValue-double-) | Устанавливает пользовательское минимальное значение для вертикальной оси. |
| [setVerticalAxisMinValue(int type, double value)](#setVerticalAxisMinValue-int-double-) | Устанавливает пользовательское минимальное значение для вертикальной оси спарклайна с указанным типом значения оси. |
| [setVerticalAxisMinValueType(int value)](#setVerticalAxisMinValueType-int-) | Представляет тип минимального значения вертикальной оси. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
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


Указывает, показывать ли данные в скрытых строках и столбцах.

**Returns:**
boolean
### getFirstPointColor() {#getFirstPointColor--}
```
public CellsColor getFirstPointColor()
```


Получает цвет первой точки данных в группе спарклайнов.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHighPointColor() {#getHighPointColor--}
```
public CellsColor getHighPointColor()
```


Получает цвет самых высоких точек данных в группе спарклайнов.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisColor() {#getHorizontalAxisColor--}
```
public CellsColor getHorizontalAxisColor()
```


Получает цвет горизонтальной оси в группе спарклайнов.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisDateRange() {#getHorizontalAxisDateRange--}
```
public String getHorizontalAxisDateRange()
```


Представляет диапазон, содержащий значения дат для данных спарклайна.

**Returns:**
java.lang.String
### getLastPointColor() {#getLastPointColor--}
```
public CellsColor getLastPointColor()
```


Получает цвет последней точки данных в группе спарклайнов.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getLineWeight() {#getLineWeight--}
```
public double getLineWeight()
```


Получает толщину линии в каждом линейном спарклайне в группе спарклайнов, в единицах пунктов.

**Returns:**
double
### getLowPointColor() {#getLowPointColor--}
```
public CellsColor getLowPointColor()
```


Получает цвет самых низких точек данных в группе спарклайнов.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getMarkersColor() {#getMarkersColor--}
```
public CellsColor getMarkersColor()
```


Получает цвет точек в каждом линейном спарклайне в группе спарклайнов.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getNegativePointsColor() {#getNegativePointsColor--}
```
public CellsColor getNegativePointsColor()
```


Получает цвет отрицательных значений в группе спарклайнов.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


Указывает, как отображать пустые ячейки.

См. [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotRightToLeft() {#getPlotRightToLeft--}
```
public boolean getPlotRightToLeft()
```


Указывает, отображаются ли данные справа налево.

**Returns:**
boolean
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


Получает тип предустановленного стиля группы спарклайнов.

См. [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

Если это свойство установлено, эти свойства: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor будут переопределены. Поэтому, пожалуйста, сначала установите это свойство, затем остальные.

**Returns:**
int
### getSeriesColor() {#getSeriesColor--}
```
public CellsColor getSeriesColor()
```


Получает цвет спарклайнов в группе спарклайнов.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getShowFirstPoint() {#getShowFirstPoint--}
```
public boolean getShowFirstPoint()
```


Указывает, выделять ли первую точку данных в группе спарклайнов.

**Returns:**
boolean
### getShowHighPoint() {#getShowHighPoint--}
```
public boolean getShowHighPoint()
```


Указывает, следует ли выделять наивысшие точки данных в группе спарклайнов.

**Returns:**
boolean
### getShowHorizontalAxis() {#getShowHorizontalAxis--}
```
public boolean getShowHorizontalAxis()
```


Указывает, следует ли отображать горизонтальную ось спарклайна. Горизонтальная ось появляется, если у спарклайна есть данные, пересекающие нулевую ось.

**Returns:**
boolean
### getShowLastPoint() {#getShowLastPoint--}
```
public boolean getShowLastPoint()
```


Указывает, следует ли выделять последнюю точку данных в группе спарклайнов.

**Returns:**
boolean
### getShowLowPoint() {#getShowLowPoint--}
```
public boolean getShowLowPoint()
```


Указывает, следует ли выделять наименьшие точки данных в группе спарклайнов.

**Returns:**
boolean
### getShowMarkers() {#getShowMarkers--}
```
public boolean getShowMarkers()
```


Указывает, следует ли выделять каждую точку в каждом линейном спарклайне в группе спарклайнов.

**Returns:**
boolean
### getShowNegativePoints() {#getShowNegativePoints--}
```
public boolean getShowNegativePoints()
```


Указывает, следует ли выделять отрицательные значения в группе спарклайнов другим цветом или маркером.

**Returns:**
boolean
### getSparklineCollection() {#getSparklineCollection--}
```
public SparklineCollection getSparklineCollection()
```


Получает коллекцию объектов [Sparkline](../../com.aspose.cells/sparkline).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство SparklineGroup.Sparklines. Это свойство будет удалено через 12 месяцев, начиная с ноября 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getSparklines() {#getSparklines--}
```
public SparklineCollection getSparklines()
```


Получает коллекцию объектов [Sparkline](../../com.aspose.cells/sparkline).

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getType() {#getType--}
```
public int getType()
```


Указывает тип спарклайна в группе спарклайнов.

См. [SparklineType](../../com.aspose.cells/sparklinetype).

**Returns:**
int
### getVerticalAxisMaxValue() {#getVerticalAxisMaxValue--}
```
public double getVerticalAxisMaxValue()
```


Получает пользовательское максимальное значение для вертикальной оси.

**Remarks**

Если это свойство установлено, [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) будет [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Returns:**
double
### getVerticalAxisMaxValueType() {#getVerticalAxisMaxValueType--}
```
public int getVerticalAxisMaxValueType()
```


Представляет тип максимального значения вертикальной оси.

См. [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Returns:**
int
### getVerticalAxisMinValue() {#getVerticalAxisMinValue--}
```
public double getVerticalAxisMinValue()
```


Получает пользовательское минимальное значение для вертикальной оси.

**Remarks**

Если это свойство установлено, [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) будет [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Returns:**
double
### getVerticalAxisMinValueType() {#getVerticalAxisMinValueType--}
```
public int getVerticalAxisMinValueType()
```


Представляет тип минимального значения вертикальной оси.

См. [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

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


Сбрасывает диапазон данных и диапазон расположения группы спарклайнов. Этот метод очистит оригинальные элементы спарклайна в группе и создаст новые элементы спарклайна для новых диапазонов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| dataRange | java.lang.String | Указывает новый диапазон данных группы спарклайнов. |
| isVertical | boolean | Указывает, следует ли строить спарклайны из нового диапазона данных по строкам или по столбцам. |
| locationRange | [CellArea](../../com.aspose.cells/cellarea) | Указывает, где разместить спарклайны. |

### setDisplayHidden(boolean value) {#setDisplayHidden-boolean-}
```
public void setDisplayHidden(boolean value)
```


Указывает, показывать ли данные в скрытых строках и столбцах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFirstPointColor(CellsColor value) {#setFirstPointColor-com.aspose.cells.CellsColor-}
```
public void setFirstPointColor(CellsColor value)
```


Устанавливает цвет первой точки данных в группе спарклайнов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHighPointColor(CellsColor value) {#setHighPointColor-com.aspose.cells.CellsColor-}
```
public void setHighPointColor(CellsColor value)
```


Устанавливает цвет наивысших точек данных в группе спарклайнов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisColor(CellsColor value) {#setHorizontalAxisColor-com.aspose.cells.CellsColor-}
```
public void setHorizontalAxisColor(CellsColor value)
```


Устанавливает цвет горизонтальной оси в группе спарклайнов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisDateRange(String value) {#setHorizontalAxisDateRange-java.lang.String-}
```
public void setHorizontalAxisDateRange(String value)
```


Представляет диапазон, содержащий значения дат для данных спарклайна.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setLastPointColor(CellsColor value) {#setLastPointColor-com.aspose.cells.CellsColor-}
```
public void setLastPointColor(CellsColor value)
```


Устанавливает цвет последней точки данных в группе спарклайнов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setLineWeight(double value) {#setLineWeight-double-}
```
public void setLineWeight(double value)
```


Устанавливает толщину линии в каждом линейном спарклайне в группе спарклайнов, в единицах точек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLowPointColor(CellsColor value) {#setLowPointColor-com.aspose.cells.CellsColor-}
```
public void setLowPointColor(CellsColor value)
```


Устанавливает цвет наименьших точек данных в группе спарклайнов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setMarkersColor(CellsColor value) {#setMarkersColor-com.aspose.cells.CellsColor-}
```
public void setMarkersColor(CellsColor value)
```


Устанавливает цвет точек в каждом линейном спарклайне в группе спарклайнов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setNegativePointsColor(CellsColor value) {#setNegativePointsColor-com.aspose.cells.CellsColor-}
```
public void setNegativePointsColor(CellsColor value)
```


Устанавливает цвет отрицательных значений в группе спарклайнов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


Указывает, как отображать пустые ячейки.

См. [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPlotRightToLeft(boolean value) {#setPlotRightToLeft-boolean-}
```
public void setPlotRightToLeft(boolean value)
```


Указывает, отображаются ли данные справа налево.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


Устанавливает тип предустановленного стиля группы спарклайнов.

См. [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

Если это свойство установлено, эти свойства: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor будут переопределены. Поэтому, пожалуйста, сначала установите это свойство, затем остальные.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSeriesColor(CellsColor value) {#setSeriesColor-com.aspose.cells.CellsColor-}
```
public void setSeriesColor(CellsColor value)
```


Устанавливает цвет спарклайнов в группе спарклайнов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setShowFirstPoint(boolean value) {#setShowFirstPoint-boolean-}
```
public void setShowFirstPoint(boolean value)
```


Указывает, выделять ли первую точку данных в группе спарклайнов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowHighPoint(boolean value) {#setShowHighPoint-boolean-}
```
public void setShowHighPoint(boolean value)
```


Указывает, следует ли выделять наивысшие точки данных в группе спарклайнов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowHorizontalAxis(boolean value) {#setShowHorizontalAxis-boolean-}
```
public void setShowHorizontalAxis(boolean value)
```


Указывает, следует ли отображать горизонтальную ось спарклайна. Горизонтальная ось появляется, если у спарклайна есть данные, пересекающие нулевую ось.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowLastPoint(boolean value) {#setShowLastPoint-boolean-}
```
public void setShowLastPoint(boolean value)
```


Указывает, следует ли выделять последнюю точку данных в группе спарклайнов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowLowPoint(boolean value) {#setShowLowPoint-boolean-}
```
public void setShowLowPoint(boolean value)
```


Указывает, следует ли выделять наименьшие точки данных в группе спарклайнов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowMarkers(boolean value) {#setShowMarkers-boolean-}
```
public void setShowMarkers(boolean value)
```


Указывает, следует ли выделять каждую точку в каждом линейном спарклайне в группе спарклайнов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowNegativePoints(boolean value) {#setShowNegativePoints-boolean-}
```
public void setShowNegativePoints(boolean value)
```


Указывает, следует ли выделять отрицательные значения в группе спарклайнов другим цветом или маркером.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Указывает тип спарклайна в группе спарклайнов.

См. [SparklineType](../../com.aspose.cells/sparklinetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setVerticalAxisMaxValue(double value) {#setVerticalAxisMaxValue-double-}
```
public void setVerticalAxisMaxValue(double value)
```


Устанавливает пользовательское максимальное значение для вертикальной оси.

**Remarks**

Если это свойство установлено, [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) будет [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setVerticalAxisMaxValue(int type, double value) {#setVerticalAxisMaxValue-int-double-}
```
public void setVerticalAxisMaxValue(int type, double value)
```


Устанавливает пользовательское максимальное значение для вертикальной оси спарклайна с указанным типом значения оси.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). Тип, определяющий, как применяется максимальное значение оси. |
| value | double | Пользовательское максимальное значение вертикальной оси. Игнорируется, если тип не [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM). |

### setVerticalAxisMaxValueType(int value) {#setVerticalAxisMaxValueType-int-}
```
public void setVerticalAxisMaxValueType(int value)
```


Представляет тип максимального значения вертикальной оси.

См. [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setVerticalAxisMinValue(double value) {#setVerticalAxisMinValue-double-}
```
public void setVerticalAxisMinValue(double value)
```


Устанавливает пользовательское минимальное значение для вертикальной оси.

**Remarks**

Если это свойство установлено, [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) будет [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setVerticalAxisMinValue(int type, double value) {#setVerticalAxisMinValue-int-double-}
```
public void setVerticalAxisMinValue(int type, double value)
```


Устанавливает пользовательское минимальное значение для вертикальной оси спарклайна с указанным типом значения оси.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). Тип, определяющий, как применяется минимальное значение оси. |
| value | double | Пользовательское минимальное значение вертикальной оси. Игнорируется, если тип не [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM). |

### setVerticalAxisMinValueType(int value) {#setVerticalAxisMinValueType-int-}
```
public void setVerticalAxisMinValueType(int value)
```


Представляет тип минимального значения вертикальной оси.

См. [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

