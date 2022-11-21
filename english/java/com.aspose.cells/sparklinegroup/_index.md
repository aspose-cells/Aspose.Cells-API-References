---
title: SparklineGroup
second_title: Aspose.Cells for Java API Reference
description: is organized into sparkline group.
type: docs
weight: 539
url: /java/com.aspose.cells/sparklinegroup/
---

**Inheritance:**
java.lang.Object
```
public class SparklineGroup
```

[Sparkline](../../com.aspose.cells/sparkline) is organized into sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

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
         int idx = sheet.getSparklineGroupCollection().add(com.aspose.cells.SparklineType.LINE, "A1:D1", false, ca);
         SparklineGroup group = sheet.getSparklineGroupCollection().get(idx);
         group.getSparklineCollection().add(sheet.getName() + "!A1:D1", 0, 4);
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
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDisplayHidden()](#getDisplayHidden--) | Indicates whether to show data in hidden rows and columns. |
| [getFirstPointColor()](#getFirstPointColor--) | Gets and sets the color of the first point of data in the sparkline group. |
| [getHighPointColor()](#getHighPointColor--) | Gets and sets the color of the highest points of data in the sparkline group. |
| [getHorizontalAxisColor()](#getHorizontalAxisColor--) | Gets and sets the color of the horizontal axis in the sparkline group. |
| [getHorizontalAxisDateRange()](#getHorizontalAxisDateRange--) | Represents the range that contains the date values for the sparkline data. |
| [getLastPointColor()](#getLastPointColor--) | Gets and sets the color of the last point of data in the sparkline group. |
| [getLineWeight()](#getLineWeight--) | Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
| [getLowPointColor()](#getLowPointColor--) | Gets and sets the color of the lowest points of data in the sparkline group. |
| [getMarkersColor()](#getMarkersColor--) | Gets and sets the color of points in each line sparkline in the sparkline group. |
| [getNegativePointsColor()](#getNegativePointsColor--) | Gets and sets the color of the negative values on the sparkline group. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Indicates how to plot empty cells. |
| [getPlotRightToLeft()](#getPlotRightToLeft--) | Indicates whether the plot data is right to left. |
| [getPresetStyle()](#getPresetStyle--) | Gets and sets the preset style type of the sparkline group. |
| [getSeriesColor()](#getSeriesColor--) | Gets and sets the color of the sparklines in the sparkline group. |
| [getShowFirstPoint()](#getShowFirstPoint--) | Indicates whether to highlight the first point of data in the sparkline group. |
| [getShowHighPoint()](#getShowHighPoint--) | Indicates whether to highlight the highest points of data in the sparkline group. |
| [getShowHorizontalAxis()](#getShowHorizontalAxis--) | Indicates whether to show the sparkline horizontal axis. |
| [getShowLastPoint()](#getShowLastPoint--) | Indicates whether to highlight the last point of data in the sparkline group. |
| [getShowLowPoint()](#getShowLowPoint--) | Indicates whether to highlight the lowest points of data in the sparkline group. |
| [getShowMarkers()](#getShowMarkers--) | Indicates whether to highlight each point in each line sparkline in the sparkline group. |
| [getShowNegativePoints()](#getShowNegativePoints--) | Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
| [getSparklineCollection()](#getSparklineCollection--) | Gets the collection of [Sparkline](../../com.aspose.cells/sparkline) object. |
| [getSparklines()](#getSparklines--) | Gets the collection of [Sparkline](../../com.aspose.cells/sparkline) object. |
| [getType()](#getType--) | Indicates the sparkline type of the sparkline group. |
| [getVerticalAxisMaxValue()](#getVerticalAxisMaxValue--) | Gets and sets the custom maximum value for the vertical axis. |
| [getVerticalAxisMaxValueType()](#getVerticalAxisMaxValueType--) | Represents the vertical axis maximum value type. |
| [getVerticalAxisMinValue()](#getVerticalAxisMinValue--) | Gets and sets the custom minimum value for the vertical axis. |
| [getVerticalAxisMinValueType()](#getVerticalAxisMinValueType--) | Represents the vertical axis minimum value type. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [resetRanges(String dataRange, boolean isVertical, CellArea locationRange)](#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-) | Resets the data range and location range of the sparkline group. |
| [setDisplayHidden(boolean value)](#setDisplayHidden-boolean-) | For the description of this property, please see [getDisplayHidden()](../../com.aspose.cells/sparklinegroup\#getDisplayHidden--) |
| [setFirstPointColor(CellsColor value)](#setFirstPointColor-com.aspose.cells.CellsColor-) | For the description of this property, please see [getFirstPointColor()](../../com.aspose.cells/sparklinegroup\#getFirstPointColor--) |
| [setHighPointColor(CellsColor value)](#setHighPointColor-com.aspose.cells.CellsColor-) | For the description of this property, please see [getHighPointColor()](../../com.aspose.cells/sparklinegroup\#getHighPointColor--) |
| [setHorizontalAxisColor(CellsColor value)](#setHorizontalAxisColor-com.aspose.cells.CellsColor-) | For the description of this property, please see [getHorizontalAxisColor()](../../com.aspose.cells/sparklinegroup\#getHorizontalAxisColor--) |
| [setHorizontalAxisDateRange(String value)](#setHorizontalAxisDateRange-java.lang.String-) | For the description of this property, please see [getHorizontalAxisDateRange()](../../com.aspose.cells/sparklinegroup\#getHorizontalAxisDateRange--) |
| [setLastPointColor(CellsColor value)](#setLastPointColor-com.aspose.cells.CellsColor-) | For the description of this property, please see [getLastPointColor()](../../com.aspose.cells/sparklinegroup\#getLastPointColor--) |
| [setLineWeight(double value)](#setLineWeight-double-) | For the description of this property, please see [getLineWeight()](../../com.aspose.cells/sparklinegroup\#getLineWeight--) |
| [setLowPointColor(CellsColor value)](#setLowPointColor-com.aspose.cells.CellsColor-) | For the description of this property, please see [getLowPointColor()](../../com.aspose.cells/sparklinegroup\#getLowPointColor--) |
| [setMarkersColor(CellsColor value)](#setMarkersColor-com.aspose.cells.CellsColor-) | For the description of this property, please see [getMarkersColor()](../../com.aspose.cells/sparklinegroup\#getMarkersColor--) |
| [setNegativePointsColor(CellsColor value)](#setNegativePointsColor-com.aspose.cells.CellsColor-) | For the description of this property, please see [getNegativePointsColor()](../../com.aspose.cells/sparklinegroup\#getNegativePointsColor--) |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | For the description of this property, please see [getPlotEmptyCellsType()](../../com.aspose.cells/sparklinegroup\#getPlotEmptyCellsType--) |
| [setPlotRightToLeft(boolean value)](#setPlotRightToLeft-boolean-) | For the description of this property, please see [getPlotRightToLeft()](../../com.aspose.cells/sparklinegroup\#getPlotRightToLeft--) |
| [setPresetStyle(int value)](#setPresetStyle-int-) | For the description of this property, please see [getPresetStyle()](../../com.aspose.cells/sparklinegroup\#getPresetStyle--) |
| [setSeriesColor(CellsColor value)](#setSeriesColor-com.aspose.cells.CellsColor-) | For the description of this property, please see [getSeriesColor()](../../com.aspose.cells/sparklinegroup\#getSeriesColor--) |
| [setShowFirstPoint(boolean value)](#setShowFirstPoint-boolean-) | For the description of this property, please see [getShowFirstPoint()](../../com.aspose.cells/sparklinegroup\#getShowFirstPoint--) |
| [setShowHighPoint(boolean value)](#setShowHighPoint-boolean-) | For the description of this property, please see [getShowHighPoint()](../../com.aspose.cells/sparklinegroup\#getShowHighPoint--) |
| [setShowHorizontalAxis(boolean value)](#setShowHorizontalAxis-boolean-) | For the description of this property, please see [getShowHorizontalAxis()](../../com.aspose.cells/sparklinegroup\#getShowHorizontalAxis--) |
| [setShowLastPoint(boolean value)](#setShowLastPoint-boolean-) | For the description of this property, please see [getShowLastPoint()](../../com.aspose.cells/sparklinegroup\#getShowLastPoint--) |
| [setShowLowPoint(boolean value)](#setShowLowPoint-boolean-) | For the description of this property, please see [getShowLowPoint()](../../com.aspose.cells/sparklinegroup\#getShowLowPoint--) |
| [setShowMarkers(boolean value)](#setShowMarkers-boolean-) | For the description of this property, please see [getShowMarkers()](../../com.aspose.cells/sparklinegroup\#getShowMarkers--) |
| [setShowNegativePoints(boolean value)](#setShowNegativePoints-boolean-) | For the description of this property, please see [getShowNegativePoints()](../../com.aspose.cells/sparklinegroup\#getShowNegativePoints--) |
| [setType(int value)](#setType-int-) | For the description of this property, please see [getType()](../../com.aspose.cells/sparklinegroup\#getType--) |
| [setVerticalAxisMaxValue(double value)](#setVerticalAxisMaxValue-double-) | For the description of this property, please see [getVerticalAxisMaxValue()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValue--) |
| [setVerticalAxisMaxValueType(int value)](#setVerticalAxisMaxValueType-int-) | For the description of this property, please see [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) |
| [setVerticalAxisMinValue(double value)](#setVerticalAxisMinValue-double-) | For the description of this property, please see [getVerticalAxisMinValue()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValue--) |
| [setVerticalAxisMinValueType(int value)](#setVerticalAxisMinValueType-int-) | For the description of this property, please see [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
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


Indicates whether to show data in hidden rows and columns.

**Returns:**
boolean
### getFirstPointColor() {#getFirstPointColor--}
```
public CellsColor getFirstPointColor()
```


Gets and sets the color of the first point of data in the sparkline group.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHighPointColor() {#getHighPointColor--}
```
public CellsColor getHighPointColor()
```


Gets and sets the color of the highest points of data in the sparkline group.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisColor() {#getHorizontalAxisColor--}
```
public CellsColor getHorizontalAxisColor()
```


Gets and sets the color of the horizontal axis in the sparkline group.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisDateRange() {#getHorizontalAxisDateRange--}
```
public String getHorizontalAxisDateRange()
```


Represents the range that contains the date values for the sparkline data.

**Returns:**
java.lang.String
### getLastPointColor() {#getLastPointColor--}
```
public CellsColor getLastPointColor()
```


Gets and sets the color of the last point of data in the sparkline group.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getLineWeight() {#getLineWeight--}
```
public double getLineWeight()
```


Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points.

**Returns:**
double
### getLowPointColor() {#getLowPointColor--}
```
public CellsColor getLowPointColor()
```


Gets and sets the color of the lowest points of data in the sparkline group.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getMarkersColor() {#getMarkersColor--}
```
public CellsColor getMarkersColor()
```


Gets and sets the color of points in each line sparkline in the sparkline group.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getNegativePointsColor() {#getNegativePointsColor--}
```
public CellsColor getNegativePointsColor()
```


Gets and sets the color of the negative values on the sparkline group.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


Indicates how to plot empty cells.

**Returns:**
int
### getPlotRightToLeft() {#getPlotRightToLeft--}
```
public boolean getPlotRightToLeft()
```


Indicates whether the plot data is right to left.

**Returns:**
boolean
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


Gets and sets the preset style type of the sparkline group.

**Returns:**
int
### getSeriesColor() {#getSeriesColor--}
```
public CellsColor getSeriesColor()
```


Gets and sets the color of the sparklines in the sparkline group.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getShowFirstPoint() {#getShowFirstPoint--}
```
public boolean getShowFirstPoint()
```


Indicates whether to highlight the first point of data in the sparkline group.

**Returns:**
boolean
### getShowHighPoint() {#getShowHighPoint--}
```
public boolean getShowHighPoint()
```


Indicates whether to highlight the highest points of data in the sparkline group.

**Returns:**
boolean
### getShowHorizontalAxis() {#getShowHorizontalAxis--}
```
public boolean getShowHorizontalAxis()
```


Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis.

**Returns:**
boolean
### getShowLastPoint() {#getShowLastPoint--}
```
public boolean getShowLastPoint()
```


Indicates whether to highlight the last point of data in the sparkline group.

**Returns:**
boolean
### getShowLowPoint() {#getShowLowPoint--}
```
public boolean getShowLowPoint()
```


Indicates whether to highlight the lowest points of data in the sparkline group.

**Returns:**
boolean
### getShowMarkers() {#getShowMarkers--}
```
public boolean getShowMarkers()
```


Indicates whether to highlight each point in each line sparkline in the sparkline group.

**Returns:**
boolean
### getShowNegativePoints() {#getShowNegativePoints--}
```
public boolean getShowNegativePoints()
```


Indicates whether to highlight the negative values on the sparkline group with a different color or marker.

**Returns:**
boolean
### getSparklineCollection() {#getSparklineCollection--}
```
public SparklineCollection getSparklineCollection()
```


Gets the collection of [Sparkline](../../com.aspose.cells/sparkline) object. NOTE: This member is now obsolete. Instead, please use SparklineGroup.Sparklines property. This property will be removed 12 months later since November 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getSparklines() {#getSparklines--}
```
public SparklineCollection getSparklines()
```


Gets the collection of [Sparkline](../../com.aspose.cells/sparkline) object.

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getType() {#getType--}
```
public int getType()
```


Indicates the sparkline type of the sparkline group.

**Returns:**
int
### getVerticalAxisMaxValue() {#getVerticalAxisMaxValue--}
```
public double getVerticalAxisMaxValue()
```


Gets and sets the custom maximum value for the vertical axis.

**Returns:**
double
### getVerticalAxisMaxValueType() {#getVerticalAxisMaxValueType--}
```
public int getVerticalAxisMaxValueType()
```


Represents the vertical axis maximum value type.

**Returns:**
int
### getVerticalAxisMinValue() {#getVerticalAxisMinValue--}
```
public double getVerticalAxisMinValue()
```


Gets and sets the custom minimum value for the vertical axis.

**Returns:**
double
### getVerticalAxisMinValueType() {#getVerticalAxisMinValueType--}
```
public int getVerticalAxisMinValueType()
```


Represents the vertical axis minimum value type.

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


Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dataRange | java.lang.String | Specifies the new data range of the sparkline group. |
| isVertical | boolean | Specifies whether to plot the sparklines from the new data range by row or by column. |
| locationRange | [CellArea](../../com.aspose.cells/cellarea) | Specifies where the sparklines to be placed. |

### setDisplayHidden(boolean value) {#setDisplayHidden-boolean-}
```
public void setDisplayHidden(boolean value)
```


For the description of this property, please see [getDisplayHidden()](../../com.aspose.cells/sparklinegroup\#getDisplayHidden--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFirstPointColor(CellsColor value) {#setFirstPointColor-com.aspose.cells.CellsColor-}
```
public void setFirstPointColor(CellsColor value)
```


For the description of this property, please see [getFirstPointColor()](../../com.aspose.cells/sparklinegroup\#getFirstPointColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHighPointColor(CellsColor value) {#setHighPointColor-com.aspose.cells.CellsColor-}
```
public void setHighPointColor(CellsColor value)
```


For the description of this property, please see [getHighPointColor()](../../com.aspose.cells/sparklinegroup\#getHighPointColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisColor(CellsColor value) {#setHorizontalAxisColor-com.aspose.cells.CellsColor-}
```
public void setHorizontalAxisColor(CellsColor value)
```


For the description of this property, please see [getHorizontalAxisColor()](../../com.aspose.cells/sparklinegroup\#getHorizontalAxisColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisDateRange(String value) {#setHorizontalAxisDateRange-java.lang.String-}
```
public void setHorizontalAxisDateRange(String value)
```


For the description of this property, please see [getHorizontalAxisDateRange()](../../com.aspose.cells/sparklinegroup\#getHorizontalAxisDateRange--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setLastPointColor(CellsColor value) {#setLastPointColor-com.aspose.cells.CellsColor-}
```
public void setLastPointColor(CellsColor value)
```


For the description of this property, please see [getLastPointColor()](../../com.aspose.cells/sparklinegroup\#getLastPointColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setLineWeight(double value) {#setLineWeight-double-}
```
public void setLineWeight(double value)
```


For the description of this property, please see [getLineWeight()](../../com.aspose.cells/sparklinegroup\#getLineWeight--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLowPointColor(CellsColor value) {#setLowPointColor-com.aspose.cells.CellsColor-}
```
public void setLowPointColor(CellsColor value)
```


For the description of this property, please see [getLowPointColor()](../../com.aspose.cells/sparklinegroup\#getLowPointColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setMarkersColor(CellsColor value) {#setMarkersColor-com.aspose.cells.CellsColor-}
```
public void setMarkersColor(CellsColor value)
```


For the description of this property, please see [getMarkersColor()](../../com.aspose.cells/sparklinegroup\#getMarkersColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setNegativePointsColor(CellsColor value) {#setNegativePointsColor-com.aspose.cells.CellsColor-}
```
public void setNegativePointsColor(CellsColor value)
```


For the description of this property, please see [getNegativePointsColor()](../../com.aspose.cells/sparklinegroup\#getNegativePointsColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


For the description of this property, please see [getPlotEmptyCellsType()](../../com.aspose.cells/sparklinegroup\#getPlotEmptyCellsType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPlotRightToLeft(boolean value) {#setPlotRightToLeft-boolean-}
```
public void setPlotRightToLeft(boolean value)
```


For the description of this property, please see [getPlotRightToLeft()](../../com.aspose.cells/sparklinegroup\#getPlotRightToLeft--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


For the description of this property, please see [getPresetStyle()](../../com.aspose.cells/sparklinegroup\#getPresetStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSeriesColor(CellsColor value) {#setSeriesColor-com.aspose.cells.CellsColor-}
```
public void setSeriesColor(CellsColor value)
```


For the description of this property, please see [getSeriesColor()](../../com.aspose.cells/sparklinegroup\#getSeriesColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setShowFirstPoint(boolean value) {#setShowFirstPoint-boolean-}
```
public void setShowFirstPoint(boolean value)
```


For the description of this property, please see [getShowFirstPoint()](../../com.aspose.cells/sparklinegroup\#getShowFirstPoint--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowHighPoint(boolean value) {#setShowHighPoint-boolean-}
```
public void setShowHighPoint(boolean value)
```


For the description of this property, please see [getShowHighPoint()](../../com.aspose.cells/sparklinegroup\#getShowHighPoint--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowHorizontalAxis(boolean value) {#setShowHorizontalAxis-boolean-}
```
public void setShowHorizontalAxis(boolean value)
```


For the description of this property, please see [getShowHorizontalAxis()](../../com.aspose.cells/sparklinegroup\#getShowHorizontalAxis--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowLastPoint(boolean value) {#setShowLastPoint-boolean-}
```
public void setShowLastPoint(boolean value)
```


For the description of this property, please see [getShowLastPoint()](../../com.aspose.cells/sparklinegroup\#getShowLastPoint--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowLowPoint(boolean value) {#setShowLowPoint-boolean-}
```
public void setShowLowPoint(boolean value)
```


For the description of this property, please see [getShowLowPoint()](../../com.aspose.cells/sparklinegroup\#getShowLowPoint--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowMarkers(boolean value) {#setShowMarkers-boolean-}
```
public void setShowMarkers(boolean value)
```


For the description of this property, please see [getShowMarkers()](../../com.aspose.cells/sparklinegroup\#getShowMarkers--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowNegativePoints(boolean value) {#setShowNegativePoints-boolean-}
```
public void setShowNegativePoints(boolean value)
```


For the description of this property, please see [getShowNegativePoints()](../../com.aspose.cells/sparklinegroup\#getShowNegativePoints--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


For the description of this property, please see [getType()](../../com.aspose.cells/sparklinegroup\#getType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setVerticalAxisMaxValue(double value) {#setVerticalAxisMaxValue-double-}
```
public void setVerticalAxisMaxValue(double value)
```


For the description of this property, please see [getVerticalAxisMaxValue()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValue--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setVerticalAxisMaxValueType(int value) {#setVerticalAxisMaxValueType-int-}
```
public void setVerticalAxisMaxValueType(int value)
```


For the description of this property, please see [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setVerticalAxisMinValue(double value) {#setVerticalAxisMinValue-double-}
```
public void setVerticalAxisMinValue(double value)
```


For the description of this property, please see [getVerticalAxisMinValue()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValue--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setVerticalAxisMinValueType(int value) {#setVerticalAxisMinValueType-int-}
```
public void setVerticalAxisMinValueType(int value)
```


For the description of this property, please see [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

