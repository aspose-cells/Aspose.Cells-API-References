---
title: ErrorBar
second_title: Aspose.Cells for Java API Reference
description: Represents error bar of data series.
type: docs
weight: 191
url: /java/com.aspose.cells/errorbar/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class ErrorBar extends Line
```

Represents error bar of data series.

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
## Constructors

| Constructor | Description |
| --- | --- |
| [ErrorBar()](#ErrorBar--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAmount()](#getAmount--) | Represents amount of error bar. |
| [getBeginArrowLength()](#getBeginArrowLength--) | Specifies the length of the arrowhead for the begin of a line. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Specifies the width of the arrowhead for the begin of a line. |
| [getBeginType()](#getBeginType--) | Specifies an arrowhead for the begin of a line. |
| [getCapType()](#getCapType--) | Specifies the ending caps. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Represents the [Color](../../com.aspose.cells/color) of the line. |
| [getCompoundType()](#getCompoundType--) | Specifies the compound line type |
| [getDashType()](#getDashType--) | Specifies the dash line type |
| [getDisplayType()](#getDisplayType--) | Represents error bar display type. |
| [getEndArrowLength()](#getEndArrowLength--) | Specifies the length of the arrowhead for the end of a line. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Specifies the width of the arrowhead for the end of a line. |
| [getEndType()](#getEndType--) | Specifies an arrowhead for the end of a line. |
| [getFormattingType()](#getFormattingType--) | Gets or sets format type. |
| [getGradientFill()](#getGradientFill--) | Represents gradient fill. |
| [getJoinType()](#getJoinType--) | Specifies the joining caps. |
| [getMinusValue()](#getMinusValue--) | Represents negative error amount when error bar type is Custom. |
| [getPlusValue()](#getPlusValue--) | Represents positive error amount when error bar type is Custom. |
| [getShowMarkerTTop()](#getShowMarkerTTop--) | Indicates if formatting error bars with a T-top. |
| [getStyle()](#getStyle--) | Represents the style of the line. |
| [getThemeColor()](#getThemeColor--) | Gets and sets the theme color. |
| [getTransparency()](#getTransparency--) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [getType()](#getType--) | Represents error bar amount type. |
| [getWeight()](#getWeight--) | Gets or sets the [WeightType](../../com.aspose.cells/weighttype) of the line. |
| [getWeightPt()](#getWeightPt--) | Gets or sets the weight of the line in unit of points. |
| [getWeightPx()](#getWeightPx--) | Gets or sets the weight of the line in unit of pixels. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Indicates whether this line style is auto assigned. |
| [isAutomaticColor()](#isAutomaticColor--) | Indicates whether the color of line is automatic assigned. |
| [isVisible()](#isVisible--) | Represents whether the line is visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAmount(double value)](#setAmount-double-) | For the description of this property, please see \#getAmount().getAmount() |
| [setAuto(boolean value)](#setAuto-boolean-) | For the description of this property, please see \#isAuto().isAuto() |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | For the description of this property, please see \#getBeginArrowLength().getBeginArrowLength() |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | For the description of this property, please see \#getBeginArrowWidth().getBeginArrowWidth() |
| [setBeginType(int value)](#setBeginType-int-) | For the description of this property, please see \#getBeginType().getBeginType() |
| [setCapType(int value)](#setCapType-int-) | For the description of this property, please see \#getCapType().getCapType() |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | For the description of this property, please see \#getColor().getColor() |
| [setCompoundType(int value)](#setCompoundType-int-) | For the description of this property, please see \#getCompoundType().getCompoundType() |
| [setDashType(int value)](#setDashType-int-) | For the description of this property, please see \#getDashType().getDashType() |
| [setDisplayType(int value)](#setDisplayType-int-) | For the description of this property, please see \#getDisplayType().getDisplayType() |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | For the description of this property, please see \#getEndArrowLength().getEndArrowLength() |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | For the description of this property, please see \#getEndArrowWidth().getEndArrowWidth() |
| [setEndType(int value)](#setEndType-int-) | For the description of this property, please see \#getEndType().getEndType() |
| [setFormattingType(int value)](#setFormattingType-int-) | For the description of this property, please see \#getFormattingType().getFormattingType() |
| [setJoinType(int value)](#setJoinType-int-) | For the description of this property, please see \#getJoinType().getJoinType() |
| [setMinusValue(String value)](#setMinusValue-java.lang.String-) | For the description of this property, please see \#getMinusValue().getMinusValue() |
| [setPlusValue(String value)](#setPlusValue-java.lang.String-) | For the description of this property, please see \#getPlusValue().getPlusValue() |
| [setShowMarkerTTop(boolean value)](#setShowMarkerTTop-boolean-) | For the description of this property, please see \#getShowMarkerTTop().getShowMarkerTTop() |
| [setStyle(int value)](#setStyle-int-) | For the description of this property, please see \#getStyle().getStyle() |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | For the description of this property, please see \#getThemeColor().getThemeColor() |
| [setTransparency(double value)](#setTransparency-double-) | For the description of this property, please see \#getTransparency().getTransparency() |
| [setType(int value)](#setType-int-) | For the description of this property, please see \#getType().getType() |
| [setVisible(boolean value)](#setVisible-boolean-) | For the description of this property, please see \#isVisible().isVisible() |
| [setWeight(int value)](#setWeight-int-) | For the description of this property, please see \#getWeight().getWeight() |
| [setWeightPt(double value)](#setWeightPt-double-) | For the description of this property, please see \#getWeightPt().getWeightPt() |
| [setWeightPx(double value)](#setWeightPx-double-) | For the description of this property, please see \#getWeightPx().getWeightPx() |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ErrorBar() {#ErrorBar--}
```
public ErrorBar()
```


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
### getAmount() {#getAmount--}
```
public double getAmount()
```


Represents amount of error bar.  The amount must be greater than or equal to zero.

**Returns:**
double
### getBeginArrowLength() {#getBeginArrowLength--}
```
public int getBeginArrowLength()
```


Specifies the length of the arrowhead for the begin of a line.

**Returns:**
int
### getBeginArrowWidth() {#getBeginArrowWidth--}
```
public int getBeginArrowWidth()
```


Specifies the width of the arrowhead for the begin of a line.

**Returns:**
int
### getBeginType() {#getBeginType--}
```
public int getBeginType()
```


Specifies an arrowhead for the begin of a line.

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


Specifies the ending caps.

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


Represents the [Color](../../com.aspose.cells/color) of the line.

**Returns:**
[Color](../../com.aspose.cells/color)
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


Specifies the compound line type

**Returns:**
int
### getDashType() {#getDashType--}
```
public int getDashType()
```


Specifies the dash line type

**Returns:**
int
### getDisplayType() {#getDisplayType--}
```
public int getDisplayType()
```


Represents error bar display type.

**Returns:**
int
### getEndArrowLength() {#getEndArrowLength--}
```
public int getEndArrowLength()
```


Specifies the length of the arrowhead for the end of a line.

**Returns:**
int
### getEndArrowWidth() {#getEndArrowWidth--}
```
public int getEndArrowWidth()
```


Specifies the width of the arrowhead for the end of a line.

**Returns:**
int
### getEndType() {#getEndType--}
```
public int getEndType()
```


Specifies an arrowhead for the end of a line.

**Returns:**
int
### getFormattingType() {#getFormattingType--}
```
public int getFormattingType()
```


Gets or sets format type.

**Returns:**
int
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Represents gradient fill.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Specifies the joining caps.

**Returns:**
int
### getMinusValue() {#getMinusValue--}
```
public String getMinusValue()
```


Represents negative error amount when error bar type is Custom.

**Returns:**
java.lang.String
### getPlusValue() {#getPlusValue--}
```
public String getPlusValue()
```


Represents positive error amount when error bar type is Custom.

**Returns:**
java.lang.String
### getShowMarkerTTop() {#getShowMarkerTTop--}
```
public boolean getShowMarkerTTop()
```


Indicates if formatting error bars with a T-top.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public int getStyle()
```


Represents the style of the line.

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Gets and sets the theme color. If the foreground color is not a theme color, NULL will be returned.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Represents error bar amount type.

```
Workbook wb = new Workbook("chart.xlsx");
         Chart chart = wb.getWorksheets().get(0).getCharts().get(0);
         Series aseries = chart.getNSeries().get(0);
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


Gets or sets the [WeightType](../../com.aspose.cells/weighttype) of the line.

**Returns:**
int
### getWeightPt() {#getWeightPt--}
```
public double getWeightPt()
```


Gets or sets the weight of the line in unit of points.

**Returns:**
double
### getWeightPx() {#getWeightPx--}
```
public double getWeightPx()
```


Gets or sets the weight of the line in unit of pixels.

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


Indicates whether this line style is auto assigned.

**Returns:**
boolean
### isAutomaticColor() {#isAutomaticColor--}
```
public boolean isAutomaticColor()
```


Indicates whether the color of line is automatic assigned.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Represents whether the line is visible.

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


For the description of this property, please see \#getAmount().getAmount()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setAuto(boolean value) {#setAuto-boolean-}
```
public void setAuto(boolean value)
```


For the description of this property, please see \#isAuto().isAuto()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBeginArrowLength(int value) {#setBeginArrowLength-int-}
```
public void setBeginArrowLength(int value)
```


For the description of this property, please see \#getBeginArrowLength().getBeginArrowLength()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBeginArrowWidth(int value) {#setBeginArrowWidth-int-}
```
public void setBeginArrowWidth(int value)
```


For the description of this property, please see \#getBeginArrowWidth().getBeginArrowWidth()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBeginType(int value) {#setBeginType-int-}
```
public void setBeginType(int value)
```


For the description of this property, please see \#getBeginType().getBeginType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


For the description of this property, please see \#getCapType().getCapType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


For the description of this property, please see \#getColor().getColor()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


For the description of this property, please see \#getCompoundType().getCompoundType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDashType(int value) {#setDashType-int-}
```
public void setDashType(int value)
```


For the description of this property, please see \#getDashType().getDashType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDisplayType(int value) {#setDisplayType-int-}
```
public void setDisplayType(int value)
```


For the description of this property, please see \#getDisplayType().getDisplayType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setEndArrowLength(int value) {#setEndArrowLength-int-}
```
public void setEndArrowLength(int value)
```


For the description of this property, please see \#getEndArrowLength().getEndArrowLength()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setEndArrowWidth(int value) {#setEndArrowWidth-int-}
```
public void setEndArrowWidth(int value)
```


For the description of this property, please see \#getEndArrowWidth().getEndArrowWidth()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setEndType(int value) {#setEndType-int-}
```
public void setEndType(int value)
```


For the description of this property, please see \#getEndType().getEndType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setFormattingType(int value) {#setFormattingType-int-}
```
public void setFormattingType(int value)
```


For the description of this property, please see \#getFormattingType().getFormattingType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


For the description of this property, please see \#getJoinType().getJoinType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMinusValue(String value) {#setMinusValue-java.lang.String-}
```
public void setMinusValue(String value)
```


For the description of this property, please see \#getMinusValue().getMinusValue()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setPlusValue(String value) {#setPlusValue-java.lang.String-}
```
public void setPlusValue(String value)
```


For the description of this property, please see \#getPlusValue().getPlusValue()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setShowMarkerTTop(boolean value) {#setShowMarkerTTop-boolean-}
```
public void setShowMarkerTTop(boolean value)
```


For the description of this property, please see \#getShowMarkerTTop().getShowMarkerTTop()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


For the description of this property, please see \#getStyle().getStyle()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


For the description of this property, please see \#getThemeColor().getThemeColor()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


For the description of this property, please see \#getTransparency().getTransparency()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


For the description of this property, please see \#getType().getType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


For the description of this property, please see \#isVisible().isVisible()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setWeight(int value) {#setWeight-int-}
```
public void setWeight(int value)
```


For the description of this property, please see \#getWeight().getWeight()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWeightPt(double value) {#setWeightPt-double-}
```
public void setWeightPt(double value)
```


For the description of this property, please see \#getWeightPt().getWeightPt()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWeightPx(double value) {#setWeightPx-double-}
```
public void setWeightPx(double value)
```


For the description of this property, please see \#getWeightPx().getWeightPx()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

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

