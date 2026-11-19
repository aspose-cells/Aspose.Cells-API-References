---
title: "ErrorBar"
second_title: "Aspose.Cells for Java API 参考"
description: "表示数据系列的误差线。"
type: docs
url: /zh/java/com.aspose.cells/errorbar/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class ErrorBar extends Line
```

表示数据系列的误差线。

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("a1").putValue(2);
         cells.get("a2").putValue(5);
         cells.get("a3").putValue(3);
         cells.get("a4").putValue(6);
         cells.get("b1").putValue(4);
         cells.get("b2").putValue(3);
         cells.get("b3").putValue(6);
         cells.get("b4").putValue(7);
 
         cells.get("C1").putValue("Q1");
         cells.get("C2").putValue("Q2");
         cells.get("C3").putValue("Y1");
         cells.get("C4").putValue("Y2");
 
         int chartIndex = workbook.getWorksheets().get(0).getCharts().add(ChartType.COLUMN, 11, 0, 27, 10);
 
         Chart chart = workbook.getWorksheets().get(0).getCharts().get(chartIndex);
         chart.getNSeries().add("A1:B4", true);
 
         chart.getNSeries().setCategoryData("C1:C4");
 
         for(int i = 0; i <chart.getNSeries().getCount(); i ++)
         {
         		Series aseries = chart.getNSeries().get(i);
         		aseries.getYErrorBar().setDisplayType(ErrorBarDisplayType.MINUS);
         		aseries.getYErrorBar().setType(ErrorBarType.FIXED_VALUE);
         		aseries.getYErrorBar().setAmount(5);
         }
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAmount()](#getAmount--) | 表示误差线的数量。 |
| [getBeginArrowLength()](#getBeginArrowLength--) | 指定线段起点的箭头长度。 |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | 指定线段起点的箭头宽度。 |
| [getBeginType()](#getBeginType--) | 指定线段起点的箭头。 |
| [getCapType()](#getCapType--) | 指定结束端帽。 |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | 表示线段的 [Color](../../com.aspose.cells/color)。 |
| [getCompoundType()](#getCompoundType--) | 指定复合线类型 |
| [getDashType()](#getDashType--) | 指定虚线类型 |
| [getDisplayType()](#getDisplayType--) | 表示误差线的显示类型。 |
| [getEndArrowLength()](#getEndArrowLength--) | 指定线段终点的箭头长度。 |
| [getEndArrowWidth()](#getEndArrowWidth--) | 指定线段终点的箭头宽度。 |
| [getEndType()](#getEndType--) | 指定线段末端的箭头。 |
| [getFormattingType()](#getFormattingType--) | 获取格式类型。 |
| [getGradientFill()](#getGradientFill--) | 表示渐变填充。 |
| [getJoinType()](#getJoinType--) | 指定连接端帽。 |
| [getMinusValue()](#getMinusValue--) | 当误差线类型为自定义时，表示负误差量。 |
| [getPlusValue()](#getPlusValue--) | 当误差线类型为自定义时，表示正误差量。 |
| [getShowMarkerTTop()](#getShowMarkerTTop--) | 指示误差线是否使用 T 型顶部进行格式化。 |
| [getStyle()](#getStyle--) | 表示线条的样式。 |
| [getThemeColor()](#getThemeColor--) | 获取主题颜色。 |
| [getTransparency()](#getTransparency--) | 返回或设置线条的透明度，取值范围为 0.0（不透明）到 1.0（透明）。 |
| [getType()](#getType--) | 表示误差线的数量类型。 |
| [getWeight()](#getWeight--) | 获取线条的 [WeightType](../../com.aspose.cells/weighttype)。 |
| [getWeightPt()](#getWeightPt--) | 获取线条的粗细，单位为磅。 |
| [getWeightPx()](#getWeightPx--) | 获取线条的粗细，单位为像素。 |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | 指示此线条样式是否自动分配。 |
| [isAutomaticColor()](#isAutomaticColor--) | 指示线条颜色是否自动分配。 |
| [isVisible()](#isVisible--) | 表示线条是否可见。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAmount(double value)](#setAmount-double-) | 表示误差线的数量。 |
| [setAuto(boolean value)](#setAuto-boolean-) | 指示此线条样式是否自动分配。 |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | 指定线段起点的箭头长度。 |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | 指定线段起点的箭头宽度。 |
| [setBeginType(int value)](#setBeginType-int-) | 指定线段起点的箭头。 |
| [setCapType(int value)](#setCapType-int-) | 指定结束端帽。 |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | 表示线段的 [Color](../../com.aspose.cells/color)。 |
| [setCompoundType(int value)](#setCompoundType-int-) | 指定复合线类型 |
| [setDashType(int value)](#setDashType-int-) | 指定虚线类型 |
| [setDisplayType(int value)](#setDisplayType-int-) | 表示误差线的显示类型。 |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | 指定线段终点的箭头长度。 |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | 指定线段终点的箭头宽度。 |
| [setEndType(int value)](#setEndType-int-) | 指定线段末端的箭头。 |
| [setFormattingType(int value)](#setFormattingType-int-) | 设置格式类型。 |
| [setJoinType(int value)](#setJoinType-int-) | 指定连接端帽。 |
| [setMinusValue(String value)](#setMinusValue-java.lang.String-) | 当误差线类型为自定义时，表示负误差量。 |
| [setPlusValue(String value)](#setPlusValue-java.lang.String-) | 当误差线类型为自定义时，表示正误差量。 |
| [setShowMarkerTTop(boolean value)](#setShowMarkerTTop-boolean-) | 指示误差线是否使用 T 型顶部进行格式化。 |
| [setStyle(int value)](#setStyle-int-) | 表示线条的样式。 |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | 设置主题颜色。 |
| [setTransparency(double value)](#setTransparency-double-) | 返回或设置线条的透明度，取值范围为 0.0（不透明）到 1.0（透明）。 |
| [setType(int value)](#setType-int-) | 表示误差线的数量类型。 |
| [setVisible(boolean value)](#setVisible-boolean-) | 表示线条是否可见。 |
| [setWeight(int value)](#setWeight-int-) | 设置线条的 [WeightType](../../com.aspose.cells/weighttype)。 |
| [setWeightPt(double value)](#setWeightPt-double-) | 设置线条的粗细，单位为点。 |
| [setWeightPx(double value)](#setWeightPx-double-) | 设置线条的粗细，单位为像素。 |
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
### getAmount() {#getAmount--}
```
public double getAmount()
```


表示误差线的数量。

**Remarks**

该数值必须大于或等于零。

**Returns:**
double
### getBeginArrowLength() {#getBeginArrowLength--}
```
public int getBeginArrowLength()
```


指定线段起点的箭头长度。

参见 [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength)。

**Returns:**
int
### getBeginArrowWidth() {#getBeginArrowWidth--}
```
public int getBeginArrowWidth()
```


指定线段起点的箭头宽度。

参见 [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth)。

**Returns:**
int
### getBeginType() {#getBeginType--}
```
public int getBeginType()
```


指定线段起点的箭头。

参见 [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle)。

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


指定结束端帽。

参见 [LineCapType](../../com.aspose.cells/linecaptype)。

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


表示线段的 [Color](../../com.aspose.cells/color)。

**Returns:**
[Color](../../com.aspose.cells/color)
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


指定复合线类型

参见 [MsoLineStyle](../../com.aspose.cells/msolinestyle)。

**Returns:**
int
### getDashType() {#getDashType--}
```
public int getDashType()
```


指定虚线类型

参见 [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle)。

**Returns:**
int
### getDisplayType() {#getDisplayType--}
```
public int getDisplayType()
```


表示误差线的显示类型。

请参阅 [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype)。

**Returns:**
int
### getEndArrowLength() {#getEndArrowLength--}
```
public int getEndArrowLength()
```


指定线段终点的箭头长度。

参见 [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength)。

**Returns:**
int
### getEndArrowWidth() {#getEndArrowWidth--}
```
public int getEndArrowWidth()
```


指定线段终点的箭头宽度。

参见 [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth)。

**Returns:**
int
### getEndType() {#getEndType--}
```
public int getEndType()
```


指定线段末端的箭头。

参见 [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle)。

**Returns:**
int
### getFormattingType() {#getFormattingType--}
```
public int getFormattingType()
```


获取格式类型。

参见 [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype)。

**Returns:**
int
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


表示渐变填充。

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


指定连接端帽。

参见 [LineJoinType](../../com.aspose.cells/linejointype)。

**Returns:**
int
### getMinusValue() {#getMinusValue--}
```
public String getMinusValue()
```


当误差线类型为自定义时，表示负误差量。

**Returns:**
java.lang.String
### getPlusValue() {#getPlusValue--}
```
public String getPlusValue()
```


当误差线类型为自定义时，表示正误差量。

**Returns:**
java.lang.String
### getShowMarkerTTop() {#getShowMarkerTTop--}
```
public boolean getShowMarkerTTop()
```


指示误差线是否使用 T 型顶部进行格式化。

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public int getStyle()
```


表示线条的样式。

参见 [LineType](../../com.aspose.cells/linetype)。

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


获取主题颜色。

**Remarks**

如果前景色不是主题颜色，将返回 NULL。

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


返回或设置线条的透明度，取值范围为 0.0（不透明）到 1.0（透明）。

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


表示误差线的数量类型。

请参阅 [ErrorBarType](../../com.aspose.cells/errorbartype)。

**Example**

```
         Workbook wb = new Workbook("chart.xlsx");
         Chart chart = wb.getWorksheets().get(0).getCharts().get(0);
         Series aseries = chart.getNSeries().get(0);
         //Gets custom error bar type
         /*ErrorBarType*/int errBarType = aseries.getYErrorBar().getType();
         //Sets custom error bar type
         aseries.getYErrorBar().setType(ErrorBarType.CUSTOM);
         aseries.getYErrorBar().setPlusValue("=Sheet1!A1");
         aseries.getYErrorBar().setMinusValue("=Sheet1!A2");
```

**Returns:**
int
### getWeight() {#getWeight--}
```
public int getWeight()
```


获取线条的 [WeightType](../../com.aspose.cells/weighttype)。

参见 [WeightType](../../com.aspose.cells/weighttype)。

**Returns:**
int
### getWeightPt() {#getWeightPt--}
```
public double getWeightPt()
```


获取线条的粗细，单位为磅。

**Returns:**
double
### getWeightPx() {#getWeightPx--}
```
public double getWeightPx()
```


获取线条的粗细，单位为像素。

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAuto() {#isAuto--}
```
public boolean isAuto()
```


指示此线条样式是否自动分配。

**Returns:**
boolean
### isAutomaticColor() {#isAutomaticColor--}
```
public boolean isAutomaticColor()
```


指示线条颜色是否自动分配。

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


表示线条是否可见。

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




### setAmount(double value) {#setAmount-double-}
```
public void setAmount(double value)
```


表示误差线的数量。

**Remarks**

该数值必须大于或等于零。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setAuto(boolean value) {#setAuto-boolean-}
```
public void setAuto(boolean value)
```


指示此线条样式是否自动分配。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBeginArrowLength(int value) {#setBeginArrowLength-int-}
```
public void setBeginArrowLength(int value)
```


指定线段起点的箭头长度。

参见 [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBeginArrowWidth(int value) {#setBeginArrowWidth-int-}
```
public void setBeginArrowWidth(int value)
```


指定线段起点的箭头宽度。

参见 [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBeginType(int value) {#setBeginType-int-}
```
public void setBeginType(int value)
```


指定线段起点的箭头。

参见 [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


指定结束端帽。

参见 [LineCapType](../../com.aspose.cells/linecaptype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


表示线段的 [Color](../../com.aspose.cells/color)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


指定复合线类型

参见 [MsoLineStyle](../../com.aspose.cells/msolinestyle)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDashType(int value) {#setDashType-int-}
```
public void setDashType(int value)
```


指定虚线类型

参见 [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDisplayType(int value) {#setDisplayType-int-}
```
public void setDisplayType(int value)
```


表示误差线的显示类型。

请参阅 [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setEndArrowLength(int value) {#setEndArrowLength-int-}
```
public void setEndArrowLength(int value)
```


指定线段终点的箭头长度。

参见 [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setEndArrowWidth(int value) {#setEndArrowWidth-int-}
```
public void setEndArrowWidth(int value)
```


指定线段终点的箭头宽度。

参见 [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setEndType(int value) {#setEndType-int-}
```
public void setEndType(int value)
```


指定线段末端的箭头。

参见 [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setFormattingType(int value) {#setFormattingType-int-}
```
public void setFormattingType(int value)
```


设置格式类型。

参见 [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


指定连接端帽。

参见 [LineJoinType](../../com.aspose.cells/linejointype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMinusValue(String value) {#setMinusValue-java.lang.String-}
```
public void setMinusValue(String value)
```


当误差线类型为自定义时，表示负误差量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPlusValue(String value) {#setPlusValue-java.lang.String-}
```
public void setPlusValue(String value)
```


当误差线类型为自定义时，表示正误差量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setShowMarkerTTop(boolean value) {#setShowMarkerTTop-boolean-}
```
public void setShowMarkerTTop(boolean value)
```


指示误差线是否使用 T 型顶部进行格式化。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


表示线条的样式。

参见 [LineType](../../com.aspose.cells/linetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


设置主题颜色。

**Remarks**

如果前景色不是主题颜色，将返回 NULL。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


返回或设置线条的透明度，取值范围为 0.0（不透明）到 1.0（透明）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


表示误差线的数量类型。

请参阅 [ErrorBarType](../../com.aspose.cells/errorbartype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


表示线条是否可见。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setWeight(int value) {#setWeight-int-}
```
public void setWeight(int value)
```


设置线条的 [WeightType](../../com.aspose.cells/weighttype)。

参见 [WeightType](../../com.aspose.cells/weighttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setWeightPt(double value) {#setWeightPt-double-}
```
public void setWeightPt(double value)
```


设置线条的粗细，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWeightPx(double value) {#setWeightPx-double-}
```
public void setWeightPx(double value)
```


设置线条的粗细，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

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

