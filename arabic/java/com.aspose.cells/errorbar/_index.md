---
title: "ErrorBar"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل شريط الخطأ لسلسلة البيانات."
type: docs
url: /ar/java/com.aspose.cells/errorbar/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class ErrorBar extends Line
```

يمثل شريط الخطأ لسلسلة البيانات.

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
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAmount()](#getAmount--) | يمثل مقدار شريط الخطأ. |
| [getBeginArrowLength()](#getBeginArrowLength--) | يحدد طول رأس السهم لبداية الخط. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | يحدد عرض رأس السهم لبداية الخط. |
| [getBeginType()](#getBeginType--) | يحدد رأس سهم لبداية الخط. |
| [getCapType()](#getCapType--) | يحدد نهايات القُبُعات. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | يمثل [Color](../../com.aspose.cells/color) للخط. |
| [getCompoundType()](#getCompoundType--) | يحدد نوع الخط المركب |
| [getDashType()](#getDashType--) | يحدد نوع الخط المتقطع |
| [getDisplayType()](#getDisplayType--) | يمثل نوع عرض شريط الخطأ. |
| [getEndArrowLength()](#getEndArrowLength--) | يحدد طول رأس السهم لنهاية الخط. |
| [getEndArrowWidth()](#getEndArrowWidth--) | يحدد عرض رأس السهم لنهاية الخط. |
| [getEndType()](#getEndType--) | يحدد رأس سهم لنهاية الخط. |
| [getFormattingType()](#getFormattingType--) | يحصل على نوع التنسيق. |
| [getGradientFill()](#getGradientFill--) | يمثل تعبئة تدرجية. |
| [getJoinType()](#getJoinType--) | يحدد قُبُعات الانضمام. |
| [getMinusValue()](#getMinusValue--) | يمثل مقدار الخطأ السالب عندما يكون نوع شريط الخطأ مخصصًا. |
| [getPlusValue()](#getPlusValue--) | يمثل مقدار الخطأ الإيجابي عندما يكون نوع شريط الخطأ مخصصًا. |
| [getShowMarkerTTop()](#getShowMarkerTTop--) | يشير إلى ما إذا كان تنسيق أشرطة الخطأ باستخدام T-top. |
| [getStyle()](#getStyle--) | يمثل نمط الخط. |
| [getThemeColor()](#getThemeColor--) | يحصل على لون السمة. |
| [getTransparency()](#getTransparency--) | يعيد أو يضبط درجة شفافية الخط كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [getType()](#getType--) | يمثل نوع مقدار شريط الخطأ. |
| [getWeight()](#getWeight--) | يحصل على [WeightType](../../com.aspose.cells/weighttype) للخط. |
| [getWeightPt()](#getWeightPt--) | يحصل على وزن الخط بوحدة النقاط. |
| [getWeightPx()](#getWeightPx--) | يحصل على وزن الخط بوحدة البكسل. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | يشير إلى ما إذا كان نمط الخط هذا مُعيّنًا تلقائيًا. |
| [isAutomaticColor()](#isAutomaticColor--) | يشير إلى ما إذا كان لون الخط مُعيّنًا تلقائيًا. |
| [isVisible()](#isVisible--) | يمثل ما إذا كان الخط مرئيًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAmount(double value)](#setAmount-double-) | يمثل مقدار شريط الخطأ. |
| [setAuto(boolean value)](#setAuto-boolean-) | يشير إلى ما إذا كان نمط الخط هذا مُعيّنًا تلقائيًا. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | يحدد طول رأس السهم لبداية الخط. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | يحدد عرض رأس السهم لبداية الخط. |
| [setBeginType(int value)](#setBeginType-int-) | يحدد رأس سهم لبداية الخط. |
| [setCapType(int value)](#setCapType-int-) | يحدد نهايات القُبُعات. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | يمثل [Color](../../com.aspose.cells/color) للخط. |
| [setCompoundType(int value)](#setCompoundType-int-) | يحدد نوع الخط المركب |
| [setDashType(int value)](#setDashType-int-) | يحدد نوع الخط المتقطع |
| [setDisplayType(int value)](#setDisplayType-int-) | يمثل نوع عرض شريط الخطأ. |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | يحدد طول رأس السهم لنهاية الخط. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | يحدد عرض رأس السهم لنهاية الخط. |
| [setEndType(int value)](#setEndType-int-) | يحدد رأس سهم لنهاية الخط. |
| [setFormattingType(int value)](#setFormattingType-int-) | يضبط نوع التنسيق. |
| [setJoinType(int value)](#setJoinType-int-) | يحدد قُبُعات الانضمام. |
| [setMinusValue(String value)](#setMinusValue-java.lang.String-) | يمثل مقدار الخطأ السالب عندما يكون نوع شريط الخطأ مخصصًا. |
| [setPlusValue(String value)](#setPlusValue-java.lang.String-) | يمثل مقدار الخطأ الإيجابي عندما يكون نوع شريط الخطأ مخصصًا. |
| [setShowMarkerTTop(boolean value)](#setShowMarkerTTop-boolean-) | يشير إلى ما إذا كان تنسيق أشرطة الخطأ باستخدام T-top. |
| [setStyle(int value)](#setStyle-int-) | يمثل نمط الخط. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | يضبط لون السمة. |
| [setTransparency(double value)](#setTransparency-double-) | يعيد أو يضبط درجة شفافية الخط كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [setType(int value)](#setType-int-) | يمثل نوع مقدار شريط الخطأ. |
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
### getAmount() {#getAmount--}
```
public double getAmount()
```


يمثل مقدار شريط الخطأ.

**Remarks**

يجب أن يكون المبلغ أكبر من أو يساوي الصفر.

**Returns:**
double
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
### getDisplayType() {#getDisplayType--}
```
public int getDisplayType()
```


يمثل نوع عرض شريط الخطأ.

انظر [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype).

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
### getMinusValue() {#getMinusValue--}
```
public String getMinusValue()
```


يمثل مقدار الخطأ السالب عندما يكون نوع شريط الخطأ مخصصًا.

**Returns:**
java.lang.String
### getPlusValue() {#getPlusValue--}
```
public String getPlusValue()
```


يمثل مقدار الخطأ الإيجابي عندما يكون نوع شريط الخطأ مخصصًا.

**Returns:**
java.lang.String
### getShowMarkerTTop() {#getShowMarkerTTop--}
```
public boolean getShowMarkerTTop()
```


يشير إلى ما إذا كان تنسيق أشرطة الخطأ باستخدام T-top.

**Returns:**
boolean
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
### getType() {#getType--}
```
public int getType()
```


يمثل نوع مقدار شريط الخطأ.

انظر [ErrorBarType](../../com.aspose.cells/errorbartype).

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




### setAmount(double value) {#setAmount-double-}
```
public void setAmount(double value)
```


يمثل مقدار شريط الخطأ.

**Remarks**

يجب أن يكون المبلغ أكبر من أو يساوي الصفر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

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

### setDisplayType(int value) {#setDisplayType-int-}
```
public void setDisplayType(int value)
```


يمثل نوع عرض شريط الخطأ.

انظر [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype).

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

### setMinusValue(String value) {#setMinusValue-java.lang.String-}
```
public void setMinusValue(String value)
```


يمثل مقدار الخطأ السالب عندما يكون نوع شريط الخطأ مخصصًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPlusValue(String value) {#setPlusValue-java.lang.String-}
```
public void setPlusValue(String value)
```


يمثل مقدار الخطأ الإيجابي عندما يكون نوع شريط الخطأ مخصصًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setShowMarkerTTop(boolean value) {#setShowMarkerTTop-boolean-}
```
public void setShowMarkerTTop(boolean value)
```


يشير إلى ما إذا كان تنسيق أشرطة الخطأ باستخدام T-top.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


يمثل نوع مقدار شريط الخطأ.

انظر [ErrorBarType](../../com.aspose.cells/errorbartype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

