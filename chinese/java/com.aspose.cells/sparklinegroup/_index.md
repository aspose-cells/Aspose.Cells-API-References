---
title: "SparklineGroup"
second_title: "Aspose.Cells for Java API 参考"
description: "被组织到一个 sparkline 组中。"
type: docs
url: /zh/java/com.aspose.cells/sparklinegroup/
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
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDisplayHidden()](#getDisplayHidden--) | 指示是否在隐藏的行和列中显示数据。 |
| [getFirstPointColor()](#getFirstPointColor--) | 获取 sparkline 组中第一个数据点的颜色。 |
| [getHighPointColor()](#getHighPointColor--) | 获取 sparkline 组中最高数据点的颜色。 |
| [getHorizontalAxisColor()](#getHorizontalAxisColor--) | 获取 sparkline 组中水平轴的颜色。 |
| [getHorizontalAxisDateRange()](#getHorizontalAxisDateRange--) | 表示包含 sparkline 数据日期值的范围。 |
| [getLastPointColor()](#getLastPointColor--) | 获取 sparkline 组中最后一个数据点的颜色。 |
| [getLineWeight()](#getLineWeight--) | 获取 sparkline 组中每个折线 sparkline 的线宽（单位为点）。 |
| [getLowPointColor()](#getLowPointColor--) | 获取 sparkline 组中最低数据点的颜色。 |
| [getMarkersColor()](#getMarkersColor--) | 获取 sparkline 组中每个折线 sparkline 的点的颜色。 |
| [getNegativePointsColor()](#getNegativePointsColor--) | 获取 sparkline 组中负值的颜色。 |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | 指示如何绘制空单元格。 |
| [getPlotRightToLeft()](#getPlotRightToLeft--) | 指示绘图数据是否从右到左。 |
| [getPresetStyle()](#getPresetStyle--) | 获取 sparkline 组的预设样式类型。 |
| [getSeriesColor()](#getSeriesColor--) | 获取 sparkline 组中 sparkline 的颜色。 |
| [getShowFirstPoint()](#getShowFirstPoint--) | 指示是否突出显示 sparkline 组中第一个数据点。 |
| [getShowHighPoint()](#getShowHighPoint--) | 指示是否在 sparkline 组中突出显示数据的最高点。 |
| [getShowHorizontalAxis()](#getShowHorizontalAxis--) | 指示是否显示 sparkline 的水平轴。 |
| [getShowLastPoint()](#getShowLastPoint--) | 指示是否在 sparkline 组中突出显示数据的最后一点。 |
| [getShowLowPoint()](#getShowLowPoint--) | 指示是否在 sparkline 组中突出显示数据的最低点。 |
| [getShowMarkers()](#getShowMarkers--) | 指示是否在 sparkline 组中的每条线 sparkline 中突出显示每个点。 |
| [getShowNegativePoints()](#getShowNegativePoints--) | 指示是否使用不同的颜色或标记突出显示 sparkline 组中的负值。 |
| [getSparklineCollection()](#getSparklineCollection--) | 获取 [Sparkline](../../com.aspose.cells/sparkline) 对象的集合。 |
| [getSparklines()](#getSparklines--) | 获取 [Sparkline](../../com.aspose.cells/sparkline) 对象的集合。 |
| [getType()](#getType--) | 指示 sparkline 组的 sparkline 类型。 |
| [getVerticalAxisMaxValue()](#getVerticalAxisMaxValue--) | 获取垂直轴的自定义最大值。 |
| [getVerticalAxisMaxValueType()](#getVerticalAxisMaxValueType--) | 表示垂直轴最大值类型。 |
| [getVerticalAxisMinValue()](#getVerticalAxisMinValue--) | 获取垂直轴的自定义最小值。 |
| [getVerticalAxisMinValueType()](#getVerticalAxisMinValueType--) | 表示垂直轴最小值类型。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [resetRanges(String dataRange, boolean isVertical, CellArea locationRange)](#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-) | 重置 sparkline 组的数据范围和位置范围。 |
| [setDisplayHidden(boolean value)](#setDisplayHidden-boolean-) | 指示是否在隐藏的行和列中显示数据。 |
| [setFirstPointColor(CellsColor value)](#setFirstPointColor-com.aspose.cells.CellsColor-) | 设置 sparkline 组中数据的第一个点的颜色。 |
| [setHighPointColor(CellsColor value)](#setHighPointColor-com.aspose.cells.CellsColor-) | 设置 sparkline 组中数据的最高点的颜色。 |
| [setHorizontalAxisColor(CellsColor value)](#setHorizontalAxisColor-com.aspose.cells.CellsColor-) | 设置 sparkline 组中水平轴的颜色。 |
| [setHorizontalAxisDateRange(String value)](#setHorizontalAxisDateRange-java.lang.String-) | 表示包含 sparkline 数据日期值的范围。 |
| [setLastPointColor(CellsColor value)](#setLastPointColor-com.aspose.cells.CellsColor-) | 设置 sparkline 组中数据的最后一点的颜色。 |
| [setLineWeight(double value)](#setLineWeight-double-) | 设置 sparkline 组中每条线 sparkline 的线宽，单位为点。 |
| [setLowPointColor(CellsColor value)](#setLowPointColor-com.aspose.cells.CellsColor-) | 设置 sparkline 组中数据的最低点的颜色。 |
| [setMarkersColor(CellsColor value)](#setMarkersColor-com.aspose.cells.CellsColor-) | 设置 sparkline 组中每条线 sparkline 的点的颜色。 |
| [setNegativePointsColor(CellsColor value)](#setNegativePointsColor-com.aspose.cells.CellsColor-) | 设置 sparkline 组中负值的颜色。 |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | 指示如何绘制空单元格。 |
| [setPlotRightToLeft(boolean value)](#setPlotRightToLeft-boolean-) | 指示绘图数据是否从右到左。 |
| [setPresetStyle(int value)](#setPresetStyle-int-) | 设置 sparkline 组的预设样式类型。 |
| [setSeriesColor(CellsColor value)](#setSeriesColor-com.aspose.cells.CellsColor-) | 设置 sparkline 组中 sparkline 的颜色。 |
| [setShowFirstPoint(boolean value)](#setShowFirstPoint-boolean-) | 指示是否突出显示 sparkline 组中第一个数据点。 |
| [setShowHighPoint(boolean value)](#setShowHighPoint-boolean-) | 指示是否在 sparkline 组中突出显示数据的最高点。 |
| [setShowHorizontalAxis(boolean value)](#setShowHorizontalAxis-boolean-) | 指示是否显示 sparkline 的水平轴。 |
| [setShowLastPoint(boolean value)](#setShowLastPoint-boolean-) | 指示是否在 sparkline 组中突出显示数据的最后一点。 |
| [setShowLowPoint(boolean value)](#setShowLowPoint-boolean-) | 指示是否在 sparkline 组中突出显示数据的最低点。 |
| [setShowMarkers(boolean value)](#setShowMarkers-boolean-) | 指示是否在 sparkline 组中的每条线 sparkline 中突出显示每个点。 |
| [setShowNegativePoints(boolean value)](#setShowNegativePoints-boolean-) | 指示是否使用不同的颜色或标记突出显示 sparkline 组中的负值。 |
| [setType(int value)](#setType-int-) | 指示 sparkline 组的 sparkline 类型。 |
| [setVerticalAxisMaxValue(double value)](#setVerticalAxisMaxValue-double-) | 设置垂直轴的自定义最大值。 |
| [setVerticalAxisMaxValue(int type, double value)](#setVerticalAxisMaxValue-int-double-) | 使用指定的轴值类型设置 sparkline 垂直轴的自定义最大值。 |
| [setVerticalAxisMaxValueType(int value)](#setVerticalAxisMaxValueType-int-) | 表示垂直轴最大值类型。 |
| [setVerticalAxisMinValue(double value)](#setVerticalAxisMinValue-double-) | 设置垂直轴的自定义最小值。 |
| [setVerticalAxisMinValue(int type, double value)](#setVerticalAxisMinValue-int-double-) | 使用指定的轴值类型设置迷你图垂直轴的自定义最小值。 |
| [setVerticalAxisMinValueType(int value)](#setVerticalAxisMinValueType-int-) | 表示垂直轴最小值类型。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
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


指示是否在隐藏的行和列中显示数据。

**Returns:**
boolean
### getFirstPointColor() {#getFirstPointColor--}
```
public CellsColor getFirstPointColor()
```


获取 sparkline 组中第一个数据点的颜色。

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHighPointColor() {#getHighPointColor--}
```
public CellsColor getHighPointColor()
```


获取 sparkline 组中最高数据点的颜色。

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisColor() {#getHorizontalAxisColor--}
```
public CellsColor getHorizontalAxisColor()
```


获取 sparkline 组中水平轴的颜色。

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisDateRange() {#getHorizontalAxisDateRange--}
```
public String getHorizontalAxisDateRange()
```


表示包含 sparkline 数据日期值的范围。

**Returns:**
java.lang.String
### getLastPointColor() {#getLastPointColor--}
```
public CellsColor getLastPointColor()
```


获取 sparkline 组中最后一个数据点的颜色。

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getLineWeight() {#getLineWeight--}
```
public double getLineWeight()
```


获取 sparkline 组中每个折线 sparkline 的线宽（单位为点）。

**Returns:**
double
### getLowPointColor() {#getLowPointColor--}
```
public CellsColor getLowPointColor()
```


获取 sparkline 组中最低数据点的颜色。

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getMarkersColor() {#getMarkersColor--}
```
public CellsColor getMarkersColor()
```


获取 sparkline 组中每个折线 sparkline 的点的颜色。

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getNegativePointsColor() {#getNegativePointsColor--}
```
public CellsColor getNegativePointsColor()
```


获取 sparkline 组中负值的颜色。

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


指示如何绘制空单元格。

参见 [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype)。

**Returns:**
int
### getPlotRightToLeft() {#getPlotRightToLeft--}
```
public boolean getPlotRightToLeft()
```


指示绘图数据是否从右到左。

**Returns:**
boolean
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


获取 sparkline 组的预设样式类型。

参见 [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype)。

**Remarks**

如果设置了此属性，这些属性：SeriesColor、NegativePointsColor、HorizontalAxisColor、MarkersColor、FirstPointColor、LastPointColor、HighPointColor、LowPointColor 将被覆盖。因此请先设置此属性，然后再设置其他属性。

**Returns:**
int
### getSeriesColor() {#getSeriesColor--}
```
public CellsColor getSeriesColor()
```


获取 sparkline 组中 sparkline 的颜色。

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getShowFirstPoint() {#getShowFirstPoint--}
```
public boolean getShowFirstPoint()
```


指示是否突出显示 sparkline 组中第一个数据点。

**Returns:**
boolean
### getShowHighPoint() {#getShowHighPoint--}
```
public boolean getShowHighPoint()
```


指示是否在 sparkline 组中突出显示数据的最高点。

**Returns:**
boolean
### getShowHorizontalAxis() {#getShowHorizontalAxis--}
```
public boolean getShowHorizontalAxis()
```


指示是否显示迷你图的水平轴。如果迷你图的数据跨越零轴，则水平轴会出现。

**Returns:**
boolean
### getShowLastPoint() {#getShowLastPoint--}
```
public boolean getShowLastPoint()
```


指示是否在 sparkline 组中突出显示数据的最后一点。

**Returns:**
boolean
### getShowLowPoint() {#getShowLowPoint--}
```
public boolean getShowLowPoint()
```


指示是否在 sparkline 组中突出显示数据的最低点。

**Returns:**
boolean
### getShowMarkers() {#getShowMarkers--}
```
public boolean getShowMarkers()
```


指示是否在 sparkline 组中的每条线 sparkline 中突出显示每个点。

**Returns:**
boolean
### getShowNegativePoints() {#getShowNegativePoints--}
```
public boolean getShowNegativePoints()
```


指示是否使用不同的颜色或标记突出显示 sparkline 组中的负值。

**Returns:**
boolean
### getSparklineCollection() {#getSparklineCollection--}
```
public SparklineCollection getSparklineCollection()
```


获取 [Sparkline](../../com.aspose.cells/sparkline) 对象的集合。

**Remarks**

注意：此成员已过时。请改用 SparklineGroup.Sparklines 属性。此属性将在自2022年11月起的12个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getSparklines() {#getSparklines--}
```
public SparklineCollection getSparklines()
```


获取 [Sparkline](../../com.aspose.cells/sparkline) 对象的集合。

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getType() {#getType--}
```
public int getType()
```


指示 sparkline 组的 sparkline 类型。

参见 [SparklineType](../../com.aspose.cells/sparklinetype)。

**Returns:**
int
### getVerticalAxisMaxValue() {#getVerticalAxisMaxValue--}
```
public double getVerticalAxisMaxValue()
```


获取垂直轴的自定义最大值。

**Remarks**

如果设置了此属性，[getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) 将为 [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM)。

**Returns:**
double
### getVerticalAxisMaxValueType() {#getVerticalAxisMaxValueType--}
```
public int getVerticalAxisMaxValueType()
```


表示垂直轴最大值类型。

参见 [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype)。

**Returns:**
int
### getVerticalAxisMinValue() {#getVerticalAxisMinValue--}
```
public double getVerticalAxisMinValue()
```


获取垂直轴的自定义最小值。

**Remarks**

如果设置了此属性，[getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) 将为 [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM)。

**Returns:**
double
### getVerticalAxisMinValueType() {#getVerticalAxisMinValueType--}
```
public int getVerticalAxisMinValueType()
```


表示垂直轴最小值类型。

参见 [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype)。

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


重置迷你图组的数据范围和位置范围。此方法将清除组中原有的迷你图项，并为新范围创建新的迷你图项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dataRange | java.lang.String | 指定迷你图组的新数据范围。 |
| isVertical | boolean | 指定是按行还是按列从新数据范围绘制迷你图。 |
| locationRange | [CellArea](../../com.aspose.cells/cellarea) | 指定迷你图的放置位置。 |

### setDisplayHidden(boolean value) {#setDisplayHidden-boolean-}
```
public void setDisplayHidden(boolean value)
```


指示是否在隐藏的行和列中显示数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFirstPointColor(CellsColor value) {#setFirstPointColor-com.aspose.cells.CellsColor-}
```
public void setFirstPointColor(CellsColor value)
```


设置 sparkline 组中数据的第一个点的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHighPointColor(CellsColor value) {#setHighPointColor-com.aspose.cells.CellsColor-}
```
public void setHighPointColor(CellsColor value)
```


设置 sparkline 组中数据的最高点的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisColor(CellsColor value) {#setHorizontalAxisColor-com.aspose.cells.CellsColor-}
```
public void setHorizontalAxisColor(CellsColor value)
```


设置 sparkline 组中水平轴的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisDateRange(String value) {#setHorizontalAxisDateRange-java.lang.String-}
```
public void setHorizontalAxisDateRange(String value)
```


表示包含 sparkline 数据日期值的范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setLastPointColor(CellsColor value) {#setLastPointColor-com.aspose.cells.CellsColor-}
```
public void setLastPointColor(CellsColor value)
```


设置 sparkline 组中数据的最后一点的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setLineWeight(double value) {#setLineWeight-double-}
```
public void setLineWeight(double value)
```


设置 sparkline 组中每条线 sparkline 的线宽，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setLowPointColor(CellsColor value) {#setLowPointColor-com.aspose.cells.CellsColor-}
```
public void setLowPointColor(CellsColor value)
```


设置 sparkline 组中数据的最低点的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setMarkersColor(CellsColor value) {#setMarkersColor-com.aspose.cells.CellsColor-}
```
public void setMarkersColor(CellsColor value)
```


设置 sparkline 组中每条线 sparkline 的点的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setNegativePointsColor(CellsColor value) {#setNegativePointsColor-com.aspose.cells.CellsColor-}
```
public void setNegativePointsColor(CellsColor value)
```


设置 sparkline 组中负值的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


指示如何绘制空单元格。

参见 [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPlotRightToLeft(boolean value) {#setPlotRightToLeft-boolean-}
```
public void setPlotRightToLeft(boolean value)
```


指示绘图数据是否从右到左。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


设置 sparkline 组的预设样式类型。

参见 [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype)。

**Remarks**

如果设置了此属性，这些属性：SeriesColor、NegativePointsColor、HorizontalAxisColor、MarkersColor、FirstPointColor、LastPointColor、HighPointColor、LowPointColor 将被覆盖。因此请先设置此属性，然后再设置其他属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSeriesColor(CellsColor value) {#setSeriesColor-com.aspose.cells.CellsColor-}
```
public void setSeriesColor(CellsColor value)
```


设置 sparkline 组中 sparkline 的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setShowFirstPoint(boolean value) {#setShowFirstPoint-boolean-}
```
public void setShowFirstPoint(boolean value)
```


指示是否突出显示 sparkline 组中第一个数据点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowHighPoint(boolean value) {#setShowHighPoint-boolean-}
```
public void setShowHighPoint(boolean value)
```


指示是否在 sparkline 组中突出显示数据的最高点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowHorizontalAxis(boolean value) {#setShowHorizontalAxis-boolean-}
```
public void setShowHorizontalAxis(boolean value)
```


指示是否显示迷你图的水平轴。如果迷你图的数据跨越零轴，则水平轴会出现。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowLastPoint(boolean value) {#setShowLastPoint-boolean-}
```
public void setShowLastPoint(boolean value)
```


指示是否在 sparkline 组中突出显示数据的最后一点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowLowPoint(boolean value) {#setShowLowPoint-boolean-}
```
public void setShowLowPoint(boolean value)
```


指示是否在 sparkline 组中突出显示数据的最低点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowMarkers(boolean value) {#setShowMarkers-boolean-}
```
public void setShowMarkers(boolean value)
```


指示是否在 sparkline 组中的每条线 sparkline 中突出显示每个点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowNegativePoints(boolean value) {#setShowNegativePoints-boolean-}
```
public void setShowNegativePoints(boolean value)
```


指示是否使用不同的颜色或标记突出显示 sparkline 组中的负值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


指示 sparkline 组的 sparkline 类型。

参见 [SparklineType](../../com.aspose.cells/sparklinetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setVerticalAxisMaxValue(double value) {#setVerticalAxisMaxValue-double-}
```
public void setVerticalAxisMaxValue(double value)
```


设置垂直轴的自定义最大值。

**Remarks**

如果设置了此属性，[getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) 将为 [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setVerticalAxisMaxValue(int type, double value) {#setVerticalAxisMaxValue-int-double-}
```
public void setVerticalAxisMaxValue(int type, double value)
```


使用指定的轴值类型设置 sparkline 垂直轴的自定义最大值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype)。指定轴最大值的应用方式的类型。 |
| value | double | 垂直轴的自定义最大值。如果类型不是 [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM)，则此值将被忽略。 |

### setVerticalAxisMaxValueType(int value) {#setVerticalAxisMaxValueType-int-}
```
public void setVerticalAxisMaxValueType(int value)
```


表示垂直轴最大值类型。

参见 [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setVerticalAxisMinValue(double value) {#setVerticalAxisMinValue-double-}
```
public void setVerticalAxisMinValue(double value)
```


设置垂直轴的自定义最小值。

**Remarks**

如果设置了此属性，[getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) 将为 [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setVerticalAxisMinValue(int type, double value) {#setVerticalAxisMinValue-int-double-}
```
public void setVerticalAxisMinValue(int type, double value)
```


使用指定的轴值类型设置迷你图垂直轴的自定义最小值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype)。指定轴最小值的应用方式的类型。 |
| value | double | 垂直轴的自定义最小值。如果类型不是 [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM)，则此值将被忽略。 |

### setVerticalAxisMinValueType(int value) {#setVerticalAxisMinValueType-int-}
```
public void setVerticalAxisMinValueType(int value)
```


表示垂直轴最小值类型。

参见 [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

