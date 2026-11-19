---
title: "SeriesLayoutProperties"
second_title: "Aspose.Cells for Java API 参考"
description: "表示系列布局的属性。"
type: docs
url: /zh/java/com.aspose.cells/serieslayoutproperties/
---

**Inheritance:**
java.lang.Object
```
public class SeriesLayoutProperties
```

表示系列布局的属性。

**Remarks**

仅适用于 BoxWhisker、Funnel、ParetoLine、Sunburst、Treemap、Waterfall 和 Histogram 图表。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SeriesLayoutProperties()](#SeriesLayoutProperties--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getMapChartProjectionType()](#getMapChartProjectionType--) | 获取地图的投影类型。 |
| [getMapChartRegionType()](#getMapChartRegionType--) | 获取地图的区域类型。 |
| [getMapLabelLayout()](#getMapLabelLayout--) | 获取地图标签的布局。 |
| [getQuartileCalculation()](#getQuartileCalculation--) | 表示系列的统计属性。 |
| [getShowConnectorLines()](#getShowConnectorLines--) | 指示是否在数据点之间显示连接线。 |
| [getShowInnerPoints()](#getShowInnerPoints--) | 指示是否显示非异常值数据点。 |
| [getShowMeanLine()](#getShowMeanLine--) | 指示是否显示连接所有均值点的线。 |
| [getShowMeanMarker()](#getShowMeanMarker--) | 指示是否显示表示均值的标记。 |
| [getShowOutlierPoints()](#getShowOutlierPoints--) | 指示是否显示异常值数据点。 |
| [getSubtotals()](#getSubtotals--) | 表示小计数据点的索引。 |
| [hashCode()](#hashCode--) |  |
| [isIntervalLeftClosed()](#isIntervalLeftClosed--) | 指示区间左侧是否闭合。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setIntervalLeftClosed(boolean value)](#setIntervalLeftClosed-boolean-) | 指示区间左侧是否闭合。 |
| [setMapChartProjectionType(int value)](#setMapChartProjectionType-int-) | 设置地图的投影类型。 |
| [setMapChartRegionType(int value)](#setMapChartRegionType-int-) | 设置地图的区域类型。 |
| [setMapLabelLayout(int value)](#setMapLabelLayout-int-) | 设置地图标签的布局。 |
| [setQuartileCalculation(int value)](#setQuartileCalculation-int-) | 表示系列的统计属性。 |
| [setShowConnectorLines(boolean value)](#setShowConnectorLines-boolean-) | 指示是否在数据点之间显示连接线。 |
| [setShowInnerPoints(boolean value)](#setShowInnerPoints-boolean-) | 指示是否显示非异常值数据点。 |
| [setShowMeanLine(boolean value)](#setShowMeanLine-boolean-) | 指示是否显示连接所有均值点的线。 |
| [setShowMeanMarker(boolean value)](#setShowMeanMarker-boolean-) | 指示是否显示表示均值的标记。 |
| [setShowOutlierPoints(boolean value)](#setShowOutlierPoints-boolean-) | 指示是否显示异常值数据点。 |
| [setSubtotals(int[] value)](#setSubtotals-int---) | 表示小计数据点的索引。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SeriesLayoutProperties() {#SeriesLayoutProperties--}
```
public SeriesLayoutProperties()
```


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
### getMapChartProjectionType() {#getMapChartProjectionType--}
```
public int getMapChartProjectionType()
```


获取地图的投影类型。

参见 [MapChartProjectionType](../../com.aspose.cells/mapchartprojectiontype)。

**Remarks**

仅适用于地图图表。

**Returns:**
int
### getMapChartRegionType() {#getMapChartRegionType--}
```
public int getMapChartRegionType()
```


获取地图的区域类型。

参见 [MapChartRegionType](../../com.aspose.cells/mapchartregiontype)。

**Remarks**

仅适用于地图图表。

**Returns:**
int
### getMapLabelLayout() {#getMapLabelLayout--}
```
public int getMapLabelLayout()
```


获取地图标签的布局。

参见 [MapChartLabelLayout](../../com.aspose.cells/mapchartlabellayout)。

**Returns:**
int
### getQuartileCalculation() {#getQuartileCalculation--}
```
public int getQuartileCalculation()
```


表示系列的统计属性。

参见 [QuartileCalculationType](../../com.aspose.cells/quartilecalculationtype)。

**Remarks**

仅适用于箱线图。

**Returns:**
int
### getShowConnectorLines() {#getShowConnectorLines--}
```
public boolean getShowConnectorLines()
```


指示是否在数据点之间显示连接线。

**Remarks**

仅适用于瀑布图。

**Returns:**
boolean
### getShowInnerPoints() {#getShowInnerPoints--}
```
public boolean getShowInnerPoints()
```


指示是否显示非异常值数据点。

**Returns:**
boolean
### getShowMeanLine() {#getShowMeanLine--}
```
public boolean getShowMeanLine()
```


指示是否显示连接所有均值点的线。

**Remarks**

仅在箱线图中有效。

**Returns:**
boolean
### getShowMeanMarker() {#getShowMeanMarker--}
```
public boolean getShowMeanMarker()
```


指示是否显示表示均值的标记。

**Returns:**
boolean
### getShowOutlierPoints() {#getShowOutlierPoints--}
```
public boolean getShowOutlierPoints()
```


指示是否显示异常值数据点。

**Returns:**
boolean
### getSubtotals() {#getSubtotals--}
```
public int[] getSubtotals()
```


表示小计数据点的索引。

**Returns:**
int[]
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isIntervalLeftClosed() {#isIntervalLeftClosed--}
```
public boolean isIntervalLeftClosed()
```


指示区间左侧是否闭合。

**Remarks**

仅适用于帕累托线图。

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




### setIntervalLeftClosed(boolean value) {#setIntervalLeftClosed-boolean-}
```
public void setIntervalLeftClosed(boolean value)
```


指示区间左侧是否闭合。

**Remarks**

仅适用于帕累托线图。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMapChartProjectionType(int value) {#setMapChartProjectionType-int-}
```
public void setMapChartProjectionType(int value)
```


设置地图的投影类型。

参见 [MapChartProjectionType](../../com.aspose.cells/mapchartprojectiontype)。

**Remarks**

仅适用于地图图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMapChartRegionType(int value) {#setMapChartRegionType-int-}
```
public void setMapChartRegionType(int value)
```


设置地图的区域类型。

参见 [MapChartRegionType](../../com.aspose.cells/mapchartregiontype)。

**Remarks**

仅适用于地图图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMapLabelLayout(int value) {#setMapLabelLayout-int-}
```
public void setMapLabelLayout(int value)
```


设置地图标签的布局。

参见 [MapChartLabelLayout](../../com.aspose.cells/mapchartlabellayout)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setQuartileCalculation(int value) {#setQuartileCalculation-int-}
```
public void setQuartileCalculation(int value)
```


表示系列的统计属性。

参见 [QuartileCalculationType](../../com.aspose.cells/quartilecalculationtype)。

**Remarks**

仅适用于箱线图。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setShowConnectorLines(boolean value) {#setShowConnectorLines-boolean-}
```
public void setShowConnectorLines(boolean value)
```


指示是否在数据点之间显示连接线。

**Remarks**

仅适用于瀑布图。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowInnerPoints(boolean value) {#setShowInnerPoints-boolean-}
```
public void setShowInnerPoints(boolean value)
```


指示是否显示非异常值数据点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowMeanLine(boolean value) {#setShowMeanLine-boolean-}
```
public void setShowMeanLine(boolean value)
```


指示是否显示连接所有均值点的线。

**Remarks**

仅在箱线图中有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowMeanMarker(boolean value) {#setShowMeanMarker-boolean-}
```
public void setShowMeanMarker(boolean value)
```


指示是否显示表示均值的标记。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowOutlierPoints(boolean value) {#setShowOutlierPoints-boolean-}
```
public void setShowOutlierPoints(boolean value)
```


指示是否显示异常值数据点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSubtotals(int[] value) {#setSubtotals-int---}
```
public void setSubtotals(int[] value)
```


表示小计数据点的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int[] |  |

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

