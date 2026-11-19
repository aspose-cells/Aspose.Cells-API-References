---
title: "ChartPoint"
second_title: "Aspose.Cells for Java API 参考"
description: "表示图表系列中的单个点。"
type: docs
url: /zh/java/com.aspose.cells/chartpoint/
---

**Inheritance:**
java.lang.Object
```
public class ChartPoint
```

表示图表系列中的单个点。

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
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArcEndPointXPx()](#getArcEndPointXPx--) | 在调用 Chart.Calculate() 方法后，获取饼图部分结束点的 x 坐标。 |
| [getArcEndPointYPx()](#getArcEndPointYPx--) | 在调用 Chart.Calculate() 方法后，获取饼图部分结束点的 y 坐标。 |
| [getArcStartPointXPx()](#getArcStartPointXPx--) | 在调用 Chart.Calculate() 方法后，获取饼图部分起始点的 x 坐标。 |
| [getArcStartPointYPx()](#getArcStartPointYPx--) | 在调用 Chart.Calculate() 方法后，获取饼图部分起始点的 y 坐标。 |
| [getArea()](#getArea--) | 获取 [getArea()](../../com.aspose.cells/chartpoint\#getArea--)。 |
| [getBorder()](#getBorder--) | 获取 [Line](../../com.aspose.cells/line)。 |
| [getBorderWidthPx()](#getBorderWidthPx--) | 在调用 Chart.Calculate() 方法后，获取边框的宽度（单位为像素）。 |
| [getBottomPointCount()](#getBottomPointCount--) | 在调用 Chart.Calculate() 方法后，获取底部点的数量。 |
| [getBottomPointXPx(int index)](#getBottomPointXPx-int-) | 在调用 Chart.Calculate() 方法后，获取形状底部点的 x 坐标。 |
| [getBottomPointYPx(int index)](#getBottomPointYPx-int-) | 在调用 Chart.Calculate() 方法后，获取形状底部点的 y 坐标。 |
| [getClass()](#getClass--) |  |
| [getDataLabels()](#getDataLabels--) | 返回一个 [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) 对象，表示与此图表点关联的数据标签。 |
| [getDoughnutInnerRadius()](#getDoughnutInnerRadius--) | 在调用 Chart.Calculate() 方法后，获取环形切片的内部半径（单位为像素）。 |
| [getEndAngle()](#getEndAngle--) | 获取饼图部分的结束角度，单位为从 x 轴顺时针测量的度数，在调用 Chart.Calculate() 方法后。 |
| [getExplosion()](#getExplosion--) | 打开的饼图切片距离饼图中心的距离以饼图直径的百分比表示。 |
| [getInnerArcEndPointXPx()](#getInnerArcEndPointXPx--) | 在调用 Chart.Calculate() 方法后，获取饼图部分结束点的 x 坐标。 |
| [getInnerArcEndPointYPx()](#getInnerArcEndPointYPx--) | 在调用 Chart.Calculate() 方法后，获取饼图部分结束点的 y 坐标。 |
| [getInnerArcStartPointXPx()](#getInnerArcStartPointXPx--) | 在调用 Chart.Calculate() 方法后，获取饼图部分起始点的 x 坐标。 |
| [getInnerArcStartPointYPx()](#getInnerArcStartPointYPx--) | 在调用 Chart.Calculate() 方法后，获取饼图部分起始点的 y 坐标。 |
| [getInnerRadiusPx()](#getInnerRadiusPx--) | 获取环形切片的内部半径（单位为像素），在调用 Chart.Calculate() 方法后。 |
| [getMarker()](#getMarker--) | 获取 [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--)。 |
| [getOnCategoryAxisPointCount()](#getOnCategoryAxisPointCount--) | 获取类别轴上点的数量，在调用 Chart.Calculate() 方法后。 |
| [getOnCategoryAxisPointXPx(int index)](#getOnCategoryAxisPointXPx-int-) | 获取类别轴上点的 x 坐标，在调用 Chart.Calculate() 方法后。 |
| [getOnCategoryAxisPointYPx(int index)](#getOnCategoryAxisPointYPx-int-) | 获取类别轴上点的 y 坐标，在调用 Chart.Calculate() 方法后。 |
| [getRadiusPx()](#getRadiusPx--) | 获取气泡、饼图或环形的半径（单位为像素），在调用 Chart.Calculate() 方法后。 |
| [getShadow()](#getShadow--) | 如果 chartpoint 有阴影，则为 true。 |
| [getShapeHeight()](#getShapeHeight--) | 获取图表高度的 1/4000 单位的高度，在调用 Chart.Calculate() 方法后。 |
| [getShapeHeightPx()](#getShapeHeightPx--) | 获取高度（单位为像素），在调用 Chart.Calculate() 方法后。 |
| [getShapeProperties()](#getShapeProperties--) | 获取保存 ChartPoint 可视形状属性的 [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) 对象。 |
| [getShapeWidth()](#getShapeWidth--) | 获取图表宽度的 1/4000 单位的宽度，在调用 Chart.Calculate() 方法后。 |
| [getShapeWidthPx()](#getShapeWidthPx--) | 获取宽度（单位为像素），在调用 Chart.Calculate() 方法后。 |
| [getShapeX()](#getShapeX--) | 获取左上角的 x 坐标，以图表宽度的 1/4000 为单位，在调用 Chart.Calculate() 方法后。 |
| [getShapeXPx()](#getShapeXPx--) | 获取左上角的 x 坐标（单位为像素），在调用 Chart.Calculate() 方法后。 |
| [getShapeY()](#getShapeY--) | 获取左上角的 y 坐标，以图表高度的 1/4000 为单位，在调用 Chart.Calculate() 方法后。 |
| [getShapeYPx()](#getShapeYPx--) | 获取左上角的 y 坐标（单位为像素），在调用 Chart.Calculate() 方法后。 |
| [getStartAngle()](#getStartAngle--) | 获取饼图部分的起始角度，单位为从 x 轴顺时针测量的度数，在调用 Chart.Calculate() 方法后。 |
| [getTopPointCount()](#getTopPointCount--) | 获取顶部点的数量，在调用 Chart.Calculate() 方法后。 |
| [getTopPointXPx(int index)](#getTopPointXPx-int-) | 获取形状顶部点的 x 坐标，在调用 Chart.Calculate() 方法后。 |
| [getTopPointYPx(int index)](#getTopPointYPx-int-) | 获取形状顶部点的 y 坐标，在调用 Chart.Calculate() 方法后。 |
| [getXValue()](#getXValue--) | 获取图表点的 X 值。 |
| [getXValueType()](#getXValueType--) | 获取图表点的 X 值类型。 |
| [getYValue()](#getYValue--) | 获取图表点的 Y 值。 |
| [getYValueType()](#getYValueType--) | 获取图表点的 Y 值类型。 |
| [hashCode()](#hashCode--) |  |
| [isInSecondaryPlot()](#isInSecondaryPlot--) | 获取一个值，指示此数据点是否位于饼形图的第二个饼或条形，或位于饼中饼或条形的饼图中。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExplosion(int value)](#setExplosion-int-) | 打开的饼图切片距离饼图中心的距离以饼图直径的百分比表示。 |
| [setInSecondaryPlot(boolean value)](#setInSecondaryPlot-boolean-) | 设置一个值，指示此数据点是否位于饼形图的第二个饼或条形，或位于饼中饼或条形的饼图中。 |
| [setShadow(boolean value)](#setShadow-boolean-) | 如果 chartpoint 有阴影，则为 true。 |
| [setXValue(Object value)](#setXValue-java.lang.Object-) | 设置图表点的 X 值。 |
| [setYValue(Object value)](#setYValue-java.lang.Object-) | 设置图表点的 Y 值。 |
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
### getArcEndPointXPx() {#getArcEndPointXPx--}
```
public float getArcEndPointXPx()
```


在调用 Chart.Calculate() 方法后，获取饼形部分结束点的 x 坐标。适用于饼图和环形图。

**Returns:**
float
### getArcEndPointYPx() {#getArcEndPointYPx--}
```
public float getArcEndPointYPx()
```


在调用 Chart.Calculate() 方法后，获取饼形部分结束点的 y 坐标。适用于饼图和环形图。

**Returns:**
float
### getArcStartPointXPx() {#getArcStartPointXPx--}
```
public float getArcStartPointXPx()
```


在调用 Chart.Calculate() 方法后，获取饼形部分起始点的 x 坐标。适用于饼图和环形图。

**Returns:**
float
### getArcStartPointYPx() {#getArcStartPointYPx--}
```
public float getArcStartPointYPx()
```


在调用 Chart.Calculate() 方法后，获取饼形部分起始点的 y 坐标。适用于饼图和环形图。

**Returns:**
float
### getArea() {#getArea--}
```
public Area getArea()
```


获取 [getArea()](../../com.aspose.cells/chartpoint\#getArea--)。

**Returns:**
[Area](../../com.aspose.cells/area)
### getBorder() {#getBorder--}
```
public Line getBorder()
```


获取 [Line](../../com.aspose.cells/line)。

**Returns:**
[Line](../../com.aspose.cells/line)
### getBorderWidthPx() {#getBorderWidthPx--}
```
public int getBorderWidthPx()
```


在调用 Chart.Calculate() 方法后，获取边框的宽度（单位为像素）。

**Returns:**
int
### getBottomPointCount() {#getBottomPointCount--}
```
public int getBottomPointCount()
```


在调用 Chart.Calculate() 方法后，获取底部点的数量。

**Returns:**
int
### getBottomPointXPx(int index) {#getBottomPointXPx-int-}
```
public float getBottomPointXPx(int index)
```


在调用 Chart.Calculate() 方法后，获取形状底部点的 x 坐标。适用于 3D 图表：Column3D、Bar3D、Cone、Cylinder、Pyramid。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

**Returns:**
float
### getBottomPointYPx(int index) {#getBottomPointYPx-int-}
```
public float getBottomPointYPx(int index)
```


在调用 Chart.Calculate() 方法后，获取形状底部点的 y 坐标。适用于 3D 图表：Column3D、Bar3D、Cone、Cylinder、Pyramid。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

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


返回一个 [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) 对象，表示与此图表点关联的数据标签。

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDoughnutInnerRadius() {#getDoughnutInnerRadius--}
```
public int getDoughnutInnerRadius()
```


在调用 Chart.Calculate() 方法后，获取环形切片的内部半径（单位为像素）。适用于环形图。

**Returns:**
int
### getEndAngle() {#getEndAngle--}
```
public float getEndAngle()
```


在调用 Chart.Calculate() 方法后，获取饼形部分的结束角度（以 x 轴顺时针方向的度数计）。适用于饼图。

**Returns:**
float
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


打开的饼图切片距离饼图中心的距离以饼图直径的百分比表示。

**Returns:**
int
### getInnerArcEndPointXPx() {#getInnerArcEndPointXPx--}
```
public float getInnerArcEndPointXPx()
```


在调用 Chart.Calculate() 方法后，获取环形图饼形部分结束点的 x 坐标。适用于环形图。

**Returns:**
float
### getInnerArcEndPointYPx() {#getInnerArcEndPointYPx--}
```
public float getInnerArcEndPointYPx()
```


在调用 Chart.Calculate() 方法后，获取环形图饼形部分结束点的 y 坐标。适用于环形图。

**Returns:**
float
### getInnerArcStartPointXPx() {#getInnerArcStartPointXPx--}
```
public float getInnerArcStartPointXPx()
```


在调用 Chart.Calculate() 方法后，获取环形图饼形部分起始点的 x 坐标。适用于环形图。

**Returns:**
float
### getInnerArcStartPointYPx() {#getInnerArcStartPointYPx--}
```
public float getInnerArcStartPointYPx()
```


在调用 Chart.Calculate() 方法后，获取环形图饼形部分起始点的 y 坐标。适用于环形图。

**Returns:**
float
### getInnerRadiusPx() {#getInnerRadiusPx--}
```
public int getInnerRadiusPx()
```


在调用 Chart.Calculate() 方法后，获取环形切片的内部半径（单位为像素）。适用于环形图。

**Remarks**

注意：此属性已过时。请改用 ChartPoint.DoughnutInnerRadius 属性。该属性将在自 2024 年 6 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


获取 [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--)。

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getOnCategoryAxisPointCount() {#getOnCategoryAxisPointCount--}
```
public int getOnCategoryAxisPointCount()
```


在调用 Chart.Calculate() 方法后，获取类别轴上的点数。仅适用于面积图。

**Remarks**

二维面积图返回 1，三维面积图返回 2。

**Returns:**
int
### getOnCategoryAxisPointXPx(int index) {#getOnCategoryAxisPointXPx-int-}
```
public float getOnCategoryAxisPointXPx(int index)
```


在调用 Chart.Calculate() 方法后，获取类别轴上点的 x 坐标。仅适用于面积图。

**Remarks**

二维面积图：索引为 0。三维面积图：索引为 0 或 1。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

**Returns:**
float
### getOnCategoryAxisPointYPx(int index) {#getOnCategoryAxisPointYPx-int-}
```
public float getOnCategoryAxisPointYPx(int index)
```


在调用 Chart.Calculate() 方法后，获取类别轴上点的 y 坐标。仅适用于面积图。

**Remarks**

二维面积图：索引为 0。三维面积图：索引为 0 或 1。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

**Returns:**
float
### getRadiusPx() {#getRadiusPx--}
```
public int getRadiusPx()
```


获取气泡、饼图或环形的半径（单位为像素），在调用 Chart.Calculate() 方法后。

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


如果 chartpoint 有阴影，则为 true。

**Returns:**
boolean
### getShapeHeight() {#getShapeHeight--}
```
public int getShapeHeight()
```


获取图表高度的 1/4000 单位的高度，在调用 Chart.Calculate() 方法后。

**Returns:**
int
### getShapeHeightPx() {#getShapeHeightPx--}
```
public int getShapeHeightPx()
```


获取高度（单位为像素），在调用 Chart.Calculate() 方法后。

**Returns:**
int
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


获取保存 ChartPoint 可视形状属性的 [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) 对象。

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShapeWidth() {#getShapeWidth--}
```
public int getShapeWidth()
```


获取图表宽度的 1/4000 单位的宽度，在调用 Chart.Calculate() 方法后。

**Returns:**
int
### getShapeWidthPx() {#getShapeWidthPx--}
```
public int getShapeWidthPx()
```


获取宽度（单位为像素），在调用 Chart.Calculate() 方法后。

**Returns:**
int
### getShapeX() {#getShapeX--}
```
public int getShapeX()
```


获取左上角的 x 坐标，以图表宽度的 1/4000 为单位，在调用 Chart.Calculate() 方法后。

**Returns:**
int
### getShapeXPx() {#getShapeXPx--}
```
public int getShapeXPx()
```


获取左上角的 x 坐标（单位为像素），在调用 Chart.Calculate() 方法后。

**Returns:**
int
### getShapeY() {#getShapeY--}
```
public int getShapeY()
```


获取左上角的 y 坐标，以图表高度的 1/4000 为单位，在调用 Chart.Calculate() 方法后。

**Returns:**
int
### getShapeYPx() {#getShapeYPx--}
```
public int getShapeYPx()
```


获取左上角的 y 坐标（单位为像素），在调用 Chart.Calculate() 方法后。

**Returns:**
int
### getStartAngle() {#getStartAngle--}
```
public float getStartAngle()
```


在调用 Chart.Calculate() 方法后，获取饼形部分的起始角度（以 x 轴顺时针方向的度数计）。适用于饼图。

**Returns:**
float
### getTopPointCount() {#getTopPointCount--}
```
public int getTopPointCount()
```


获取顶部点的数量，在调用 Chart.Calculate() 方法后。

**Returns:**
int
### getTopPointXPx(int index) {#getTopPointXPx-int-}
```
public float getTopPointXPx(int index)
```


在调用 Chart.Calculate() 方法后获取形状顶部点的 X 坐标。适用于 3D 图表：Column3D、Bar3D、Cone、Cylinder、Pyramid 和 Area3D

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

**Returns:**
float
### getTopPointYPx(int index) {#getTopPointYPx-int-}
```
public float getTopPointYPx(int index)
```


在调用 Chart.Calculate() 方法后获取形状顶部点的 Y 坐标。适用于 3D 图表：Column3D、Bar3D、Cone、Cylinder、Pyramid 和 Area3D。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

**Returns:**
float
### getXValue() {#getXValue--}
```
public Object getXValue()
```


获取图表点的 X 值。

**Returns:**
java.lang.Object
### getXValueType() {#getXValueType--}
```
public int getXValueType()
```


获取图表点的 X 值类型。

参见 [CellValueType](../../com.aspose.cells/cellvaluetype)。

**Returns:**
int
### getYValue() {#getYValue--}
```
public Object getYValue()
```


获取图表点的 Y 值。

**Returns:**
java.lang.Object
### getYValueType() {#getYValueType--}
```
public int getYValueType()
```


获取图表点的 Y 值类型。

参见 [CellValueType](../../com.aspose.cells/cellvaluetype)。

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


获取一个值，指示此数据点是否位于饼形图的第二个饼或条形，或位于饼中饼或条形的饼图中。

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


打开的饼图切片距离饼图中心的距离以饼图直径的百分比表示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setInSecondaryPlot(boolean value) {#setInSecondaryPlot-boolean-}
```
public void setInSecondaryPlot(boolean value)
```


设置一个值，指示此数据点是否位于饼形图的第二个饼或条形，或位于饼中饼或条形的饼图中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


如果 chartpoint 有阴影，则为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setXValue(Object value) {#setXValue-java.lang.Object-}
```
public void setXValue(Object value)
```


设置图表点的 X 值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

### setYValue(Object value) {#setYValue-java.lang.Object-}
```
public void setYValue(Object value)
```


设置图表点的 Y 值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

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

