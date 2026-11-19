---
title: "Line"
second_title: "Aspose.Cells for Java API Reference"
description: "يغلف الكائن الذي يمثل تنسيق الخط."
type: docs
url: /ar/java/com.aspose.cells/line/
---

**Inheritance:**
java.lang.Object
```
public class Line
```

يغلف الكائن الذي يمثل تنسيق الخط.

**Example**

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
 
         	int chartIndex = sheet.getCharts().add(ChartType.LINE, 9, 9, 21, 15);
         Chart chart = sheet.getCharts().get(chartIndex);
         //Add series
         chart.getNSeries().add("A2:B4", true);
         //Set category data
         chart.getNSeries().setCategoryData("=Sheet1!$A$2:$A$4");
         //Applying a dotted line style on the lines of an NSeries
         chart.getNSeries().get(0).getBorder().setStyle(LineType.DOT);
         chart.getNSeries().get(0).getBorder().setColor(Color.getRed());
         //Applying a triangular marker style on the data markers of an NSeries
         chart.getNSeries().get(0).getMarker().setMarkerStyle(ChartMarkerType.TRIANGLE);
         //Setting the weight of all lines in an NSeries to medium
         chart.getNSeries().get(0).getBorder().setWeight(WeightType.MEDIUM_LINE);
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBeginArrowLength()](#getBeginArrowLength--) | يحدد طول رأس السهم لبداية الخط. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | يحدد عرض رأس السهم لبداية الخط. |
| [getBeginType()](#getBeginType--) | يحدد رأس سهم لبداية الخط. |
| [getCapType()](#getCapType--) | يحدد نهايات القُبُعات. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | يمثل [Color](../../com.aspose.cells/color) للخط. |
| [getCompoundType()](#getCompoundType--) | يحدد نوع الخط المركب |
| [getDashType()](#getDashType--) | يحدد نوع الخط المتقطع |
| [getEndArrowLength()](#getEndArrowLength--) | يحدد طول رأس السهم لنهاية الخط. |
| [getEndArrowWidth()](#getEndArrowWidth--) | يحدد عرض رأس السهم لنهاية الخط. |
| [getEndType()](#getEndType--) | يحدد رأس سهم لنهاية الخط. |
| [getFormattingType()](#getFormattingType--) | يحصل على نوع التنسيق. |
| [getGradientFill()](#getGradientFill--) | يمثل تعبئة تدرجية. |
| [getJoinType()](#getJoinType--) | يحدد قُبُعات الانضمام. |
| [getStyle()](#getStyle--) | يمثل نمط الخط. |
| [getThemeColor()](#getThemeColor--) | يحصل على لون السمة. |
| [getTransparency()](#getTransparency--) | يعيد أو يضبط درجة شفافية الخط كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [getWeight()](#getWeight--) | يحصل على [WeightType](../../com.aspose.cells/weighttype) للخط. |
| [getWeightPt()](#getWeightPt--) | يحصل على وزن الخط بوحدة النقاط. |
| [getWeightPx()](#getWeightPx--) | يحصل على وزن الخط بوحدة البكسل. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | يشير إلى ما إذا كان نمط الخط هذا مُعيّنًا تلقائيًا. |
| [isAutomaticColor()](#isAutomaticColor--) | يشير إلى ما إذا كان لون الخط مُعيّنًا تلقائيًا. |
| [isVisible()](#isVisible--) | يمثل ما إذا كان الخط مرئيًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | يشير إلى ما إذا كان نمط الخط هذا مُعيّنًا تلقائيًا. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | يحدد طول رأس السهم لبداية الخط. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | يحدد عرض رأس السهم لبداية الخط. |
| [setBeginType(int value)](#setBeginType-int-) | يحدد رأس سهم لبداية الخط. |
| [setCapType(int value)](#setCapType-int-) | يحدد نهايات القُبُعات. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | يمثل [Color](../../com.aspose.cells/color) للخط. |
| [setCompoundType(int value)](#setCompoundType-int-) | يحدد نوع الخط المركب |
| [setDashType(int value)](#setDashType-int-) | يحدد نوع الخط المتقطع |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | يحدد طول رأس السهم لنهاية الخط. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | يحدد عرض رأس السهم لنهاية الخط. |
| [setEndType(int value)](#setEndType-int-) | يحدد رأس سهم لنهاية الخط. |
| [setFormattingType(int value)](#setFormattingType-int-) | يضبط نوع التنسيق. |
| [setJoinType(int value)](#setJoinType-int-) | يحدد قُبُعات الانضمام. |
| [setStyle(int value)](#setStyle-int-) | يمثل نمط الخط. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | يضبط لون السمة. |
| [setTransparency(double value)](#setTransparency-double-) | يعيد أو يضبط درجة شفافية الخط كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [setVisible(boolean value)](#setVisible-boolean-) | يمثل ما إذا كان الخط مرئيًا. |
| [setWeight(int value)](#setWeight-int-) | يضبط [WeightType](../../com.aspose.cells/weighttype) للخط. |
| [setWeightPt(double value)](#setWeightPt-double-) | يضبط وزن الخط بوحدة النقاط. |
| [setWeightPx(double value)](#setWeightPx-double-) | يضبط وزن الخط بوحدة البكسل. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBeginArrowLength() {#getBeginArrowLength--}
```
public int getBeginArrowLength()
```


يحدد طول رأس السهم لبداية الخط.

انظر [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getBeginArrowWidth() {#getBeginArrowWidth--}
```
public int getBeginArrowWidth()
```


يحدد عرض رأس السهم لبداية الخط.

انظر [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getBeginType() {#getBeginType--}
```
public int getBeginType()
```


يحدد رأس سهم لبداية الخط.

انظر [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


يحدد نهايات القُبُعات.

انظر [LineCapType](../../com.aspose.cells/linecaptype).

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


يمثل [Color](../../com.aspose.cells/color) للخط.

**Returns:**
[Color](../../com.aspose.cells/color)
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


يحدد نوع الخط المركب

انظر [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Returns:**
int
### getDashType() {#getDashType--}
```
public int getDashType()
```


يحدد نوع الخط المتقطع

انظر [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Returns:**
int
### getEndArrowLength() {#getEndArrowLength--}
```
public int getEndArrowLength()
```


يحدد طول رأس السهم لنهاية الخط.

انظر [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getEndArrowWidth() {#getEndArrowWidth--}
```
public int getEndArrowWidth()
```


يحدد عرض رأس السهم لنهاية الخط.

انظر [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getEndType() {#getEndType--}
```
public int getEndType()
```


يحدد رأس سهم لنهاية الخط.

انظر [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getFormattingType() {#getFormattingType--}
```
public int getFormattingType()
```


يحصل على نوع التنسيق.

انظر [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Returns:**
int
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


يمثل تعبئة تدرجية.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


يحدد قُبُعات الانضمام.

انظر [LineJoinType](../../com.aspose.cells/linejointype).

**Returns:**
int
### getStyle() {#getStyle--}
```
public int getStyle()
```


يمثل نمط الخط.

انظر [LineType](../../com.aspose.cells/linetype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


يحصل على لون السمة.

**Remarks**

إذا لم يكن لون المقدمة لونًا من السمة، سيتم إرجاع NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


يعيد أو يضبط درجة شفافية الخط كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

**Returns:**
double
### getWeight() {#getWeight--}
```
public int getWeight()
```


يحصل على [WeightType](../../com.aspose.cells/weighttype) للخط.

انظر [WeightType](../../com.aspose.cells/weighttype).

**Returns:**
int
### getWeightPt() {#getWeightPt--}
```
public double getWeightPt()
```


يحصل على وزن الخط بوحدة النقاط.

**Returns:**
double
### getWeightPx() {#getWeightPx--}
```
public double getWeightPx()
```


يحصل على وزن الخط بوحدة البكسل.

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


يشير إلى ما إذا كان نمط الخط هذا مُعيّنًا تلقائيًا.

**Returns:**
boolean
### isAutomaticColor() {#isAutomaticColor--}
```
public boolean isAutomaticColor()
```


يشير إلى ما إذا كان لون الخط مُعيّنًا تلقائيًا.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


يمثل ما إذا كان الخط مرئيًا.

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




### setAuto(boolean value) {#setAuto-boolean-}
```
public void setAuto(boolean value)
```


يشير إلى ما إذا كان نمط الخط هذا مُعيّنًا تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBeginArrowLength(int value) {#setBeginArrowLength-int-}
```
public void setBeginArrowLength(int value)
```


يحدد طول رأس السهم لبداية الخط.

انظر [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBeginArrowWidth(int value) {#setBeginArrowWidth-int-}
```
public void setBeginArrowWidth(int value)
```


يحدد عرض رأس السهم لبداية الخط.

انظر [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBeginType(int value) {#setBeginType-int-}
```
public void setBeginType(int value)
```


يحدد رأس سهم لبداية الخط.

انظر [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


يحدد نهايات القُبُعات.

انظر [LineCapType](../../com.aspose.cells/linecaptype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


يمثل [Color](../../com.aspose.cells/color) للخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


يحدد نوع الخط المركب

انظر [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDashType(int value) {#setDashType-int-}
```
public void setDashType(int value)
```


يحدد نوع الخط المتقطع

انظر [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setEndArrowLength(int value) {#setEndArrowLength-int-}
```
public void setEndArrowLength(int value)
```


يحدد طول رأس السهم لنهاية الخط.

انظر [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setEndArrowWidth(int value) {#setEndArrowWidth-int-}
```
public void setEndArrowWidth(int value)
```


يحدد عرض رأس السهم لنهاية الخط.

انظر [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setEndType(int value) {#setEndType-int-}
```
public void setEndType(int value)
```


يحدد رأس سهم لنهاية الخط.

انظر [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setFormattingType(int value) {#setFormattingType-int-}
```
public void setFormattingType(int value)
```


يضبط نوع التنسيق.

انظر [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


يحدد قُبُعات الانضمام.

انظر [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


يمثل نمط الخط.

انظر [LineType](../../com.aspose.cells/linetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


يضبط لون السمة.

**Remarks**

إذا لم يكن لون المقدمة لونًا من السمة، سيتم إرجاع NULL.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


يعيد أو يضبط درجة شفافية الخط كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


يمثل ما إذا كان الخط مرئيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setWeight(int value) {#setWeight-int-}
```
public void setWeight(int value)
```


يضبط [WeightType](../../com.aspose.cells/weighttype) للخط.

انظر [WeightType](../../com.aspose.cells/weighttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setWeightPt(double value) {#setWeightPt-double-}
```
public void setWeightPt(double value)
```


يضبط وزن الخط بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWeightPx(double value) {#setWeightPx-double-}
```
public void setWeightPx(double value)
```


يضبط وزن الخط بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

