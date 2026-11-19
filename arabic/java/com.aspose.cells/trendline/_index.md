---
title: "Trendline"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خط الاتجاه في مخطط."
type: docs
url: /ar/java/com.aspose.cells/trendline/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class Trendline extends Line
```

يمثل خط الاتجاه في مخطط.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         //adding a linear trendline
         int index = chart.getNSeries().get(0).getTrendLines().add(TrendlineType.LINEAR);
         Trendline trendline = chart.getNSeries().get(0).getTrendLines().get(index);
         //Setting the custom name of the trendline.
         trendline.setName("Linear");
         //Displaying the equation on chart
         trendline.setDisplayEquation(true);
         //Displaying the R-Squared value on chart
         trendline.setDisplayRSquared(true);
         //Saving the Excel file
         workbook.save("book1.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackward()](#getBackward--) | يعيد أو يضبط عدد الفترات (أو الوحدات في مخطط مبعثر) التي يمتد فيها خط الاتجاه إلى الخلف. |
| [getBeginArrowLength()](#getBeginArrowLength--) | يحدد طول رأس السهم لبداية الخط. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | يحدد عرض رأس السهم لبداية الخط. |
| [getBeginType()](#getBeginType--) | يحدد رأس سهم لبداية الخط. |
| [getCapType()](#getCapType--) | يحدد نهايات القُبُعات. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | يمثل [Color](../../com.aspose.cells/color) للخط. |
| [getCompoundType()](#getCompoundType--) | يحدد نوع الخط المركب |
| [getDashType()](#getDashType--) | يحدد نوع الخط المتقطع |
| [getDataLabels()](#getDataLabels--) | يمثل كائن DataLabels للسلسلة المحددة. |
| [getDisplayEquation()](#getDisplayEquation--) | يمثل ما إذا كانت معادلة خط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كقيمة R-squared). |
| [getDisplayRSquared()](#getDisplayRSquared--) | يمثل ما إذا كانت قيمة R-squared لخط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كالمعادلة). |
| [getEndArrowLength()](#getEndArrowLength--) | يحدد طول رأس السهم لنهاية الخط. |
| [getEndArrowWidth()](#getEndArrowWidth--) | يحدد عرض رأس السهم لنهاية الخط. |
| [getEndType()](#getEndType--) | يحدد رأس سهم لنهاية الخط. |
| [getFormattingType()](#getFormattingType--) | يحصل على نوع التنسيق. |
| [getForward()](#getForward--) | يعيد أو يضبط عدد الفترات (أو الوحدات في مخطط التبعثر) التي يمتد إليها خط الاتجاه إلى الأمام. |
| [getGradientFill()](#getGradientFill--) | يمثل تعبئة تدرجية. |
| [getIntercept()](#getIntercept--) | يعيد أو يضبط النقطة التي يقطع فيها خط الاتجاه محور القيم. |
| [getJoinType()](#getJoinType--) | يحدد قُبُعات الانضمام. |
| [getLegendEntry()](#getLegendEntry--) | يحصل على مدخل الأسطورة وفقًا لهذا خط الاتجاه |
| [getName()](#getName--) | يعيد اسم خط الاتجاه. |
| [getOrder()](#getOrder--) | يعيد أو يضبط ترتيب خط الاتجاه (عدد صحيح أكبر من 1) عندما يكون نوع خط الاتجاه متعدد الحدود. |
| [getPeriod()](#getPeriod--) | يعيد أو يضبط الفترة لخط الاتجاه المتوسط المتحرك. |
| [getStyle()](#getStyle--) | يمثل نمط الخط. |
| [getThemeColor()](#getThemeColor--) | يحصل على لون السمة. |
| [getTransparency()](#getTransparency--) | يعيد أو يضبط درجة شفافية الخط كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [getType()](#getType--) | يعيد نوع خط الاتجاه. |
| [getWeight()](#getWeight--) | يحصل على [WeightType](../../com.aspose.cells/weighttype) للخط. |
| [getWeightPt()](#getWeightPt--) | يحصل على وزن الخط بوحدة النقاط. |
| [getWeightPx()](#getWeightPx--) | يحصل على وزن الخط بوحدة البكسل. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | يشير إلى ما إذا كان نمط الخط هذا مُعيّنًا تلقائيًا. |
| [isAutomaticColor()](#isAutomaticColor--) | يشير إلى ما إذا كان لون الخط مُعيّنًا تلقائيًا. |
| [isInterceptAuto()](#isInterceptAuto--) | يشير إلى ما إذا كان Microsoft Workbook يحدد تلقائيًا تقاطع خط الاتجاه. |
| [isNameAuto()](#isNameAuto--) | يعيد ما إذا كان Microsoft Excel يحدد تلقائيًا اسم خط الاتجاه. |
| [isVisible()](#isVisible--) | يمثل ما إذا كان الخط مرئيًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | يشير إلى ما إذا كان نمط الخط هذا مُعيّنًا تلقائيًا. |
| [setBackward(double value)](#setBackward-double-) | يعيد أو يضبط عدد الفترات (أو الوحدات في مخطط مبعثر) التي يمتد فيها خط الاتجاه إلى الخلف. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | يحدد طول رأس السهم لبداية الخط. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | يحدد عرض رأس السهم لبداية الخط. |
| [setBeginType(int value)](#setBeginType-int-) | يحدد رأس سهم لبداية الخط. |
| [setCapType(int value)](#setCapType-int-) | يحدد نهايات القُبُعات. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | يمثل [Color](../../com.aspose.cells/color) للخط. |
| [setCompoundType(int value)](#setCompoundType-int-) | يحدد نوع الخط المركب |
| [setDashType(int value)](#setDashType-int-) | يحدد نوع الخط المتقطع |
| [setDisplayEquation(boolean value)](#setDisplayEquation-boolean-) | يمثل ما إذا كانت معادلة خط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كقيمة R-squared). |
| [setDisplayRSquared(boolean value)](#setDisplayRSquared-boolean-) | يمثل ما إذا كانت قيمة R-squared لخط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كالمعادلة). |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | يحدد طول رأس السهم لنهاية الخط. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | يحدد عرض رأس السهم لنهاية الخط. |
| [setEndType(int value)](#setEndType-int-) | يحدد رأس سهم لنهاية الخط. |
| [setFormattingType(int value)](#setFormattingType-int-) | يضبط نوع التنسيق. |
| [setForward(double value)](#setForward-double-) | يعيد أو يضبط عدد الفترات (أو الوحدات في مخطط التبعثر) التي يمتد إليها خط الاتجاه إلى الأمام. |
| [setIntercept(double value)](#setIntercept-double-) | يعيد أو يضبط النقطة التي يقطع فيها خط الاتجاه محور القيم. |
| [setInterceptAuto(boolean isInterceptAuto)](#setInterceptAuto-boolean-) | يضبط ما إذا كان Microsoft Workbook يحدد تلقائيًا تقاطع خط الاتجاه. |
| [setJoinType(int value)](#setJoinType-int-) | يحدد قُبُعات الانضمام. |
| [setName(String value)](#setName-java.lang.String-) | يعيد اسم خط الاتجاه. |
| [setNameAuto(boolean value)](#setNameAuto-boolean-) | يعيد ما إذا كان Microsoft Excel يحدد تلقائيًا اسم خط الاتجاه. |
| [setOrder(int value)](#setOrder-int-) | يعيد أو يضبط ترتيب خط الاتجاه (عدد صحيح أكبر من 1) عندما يكون نوع خط الاتجاه متعدد الحدود. |
| [setPeriod(int value)](#setPeriod-int-) | يعيد أو يضبط الفترة لخط الاتجاه المتوسط المتحرك. |
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
### getBackward() {#getBackward--}
```
public double getBackward()
```


يعيد أو يضبط عدد الفترات (أو الوحدات في مخطط مبعثر) التي يمتد فيها خط الاتجاه إلى الخلف. يجب أن يكون عدد الفترات أكبر من أو يساوي الصفر. إذا كان نوع المخطط عموديًا، يجب أن يكون عدد الفترات بين 0 و 0.5

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
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


يمثل كائن DataLabels للسلسلة المحددة.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayEquation() {#getDisplayEquation--}
```
public boolean getDisplayEquation()
```


يمثل ما إذا كانت معادلة خط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كقيمة R‑squared). ضبط هذه الخاصية على True يُفعّل تلقائيًا تسميات البيانات.

**Returns:**
boolean
### getDisplayRSquared() {#getDisplayRSquared--}
```
public boolean getDisplayRSquared()
```


يمثل ما إذا كانت قيمة R‑squared لخط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كالمعادلة). ضبط هذه الخاصية على True يُفعّل تلقائيًا تسميات البيانات.

**Returns:**
boolean
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
### getForward() {#getForward--}
```
public double getForward()
```


يعيد أو يضبط عدد الفترات (أو الوحدات في مخطط مبعثر) التي يمتد فيها خط الاتجاه إلى الأمام. يجب أن يكون عدد الفترات أكبر من أو يساوي الصفر.

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


يمثل تعبئة تدرجية.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getIntercept() {#getIntercept--}
```
public double getIntercept()
```


يعيد أو يضبط النقطة التي يقطع فيها خط الاتجاه محور القيم.

**Returns:**
double
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


يحدد قُبُعات الانضمام.

انظر [LineJoinType](../../com.aspose.cells/linejointype).

**Returns:**
int
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


يحصل على مدخل الأسطورة وفقًا لهذا خط الاتجاه

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getName() {#getName--}
```
public String getName()
```


يعيد اسم خط الاتجاه.

**Returns:**
java.lang.String
### getOrder() {#getOrder--}
```
public int getOrder()
```


يعيد أو يضبط ترتيب خط الاتجاه (عدد صحيح أكبر من 1) عندما يكون نوع خط الاتجاه متعدد الحدود. يجب أن يكون الترتيب بين 2 و 6.

**Returns:**
int
### getPeriod() {#getPeriod--}
```
public int getPeriod()
```


يعيد أو يضبط الفترة لخط الاتجاه المتوسط المتحرك.

**Remarks**

يجب أن تكون هذه القيمة بين 2 و 255. ويجب أن تكون أقل من عدد نقاط المخطط في السلسلة

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
### getType() {#getType--}
```
public int getType()
```


يعيد نوع خط الاتجاه.

انظر [TrendlineType](../../com.aspose.cells/trendlinetype).

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
### isInterceptAuto() {#isInterceptAuto--}
```
public boolean isInterceptAuto()
```


يشير إلى ما إذا كان Microsoft Workbook يحدد تلقائيًا تقاطع خط الاتجاه.

**Returns:**
boolean
### isNameAuto() {#isNameAuto--}
```
public boolean isNameAuto()
```


يعيد ما إذا كان Microsoft Excel يحدد تلقائيًا اسم خط الاتجاه.

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

### setBackward(double value) {#setBackward-double-}
```
public void setBackward(double value)
```


يعيد أو يضبط عدد الفترات (أو الوحدات في مخطط مبعثر) التي يمتد فيها خط الاتجاه إلى الخلف. يجب أن يكون عدد الفترات أكبر من أو يساوي الصفر. إذا كان نوع المخطط عموديًا، يجب أن يكون عدد الفترات بين 0 و 0.5

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

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

### setDisplayEquation(boolean value) {#setDisplayEquation-boolean-}
```
public void setDisplayEquation(boolean value)
```


يمثل ما إذا كانت معادلة خط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كقيمة R‑squared). ضبط هذه الخاصية على True يُفعّل تلقائيًا تسميات البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDisplayRSquared(boolean value) {#setDisplayRSquared-boolean-}
```
public void setDisplayRSquared(boolean value)
```


يمثل ما إذا كانت قيمة R‑squared لخط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كالمعادلة). ضبط هذه الخاصية على True يُفعّل تلقائيًا تسميات البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

### setForward(double value) {#setForward-double-}
```
public void setForward(double value)
```


يعيد أو يضبط عدد الفترات (أو الوحدات في مخطط مبعثر) التي يمتد فيها خط الاتجاه إلى الأمام. يجب أن يكون عدد الفترات أكبر من أو يساوي الصفر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setIntercept(double value) {#setIntercept-double-}
```
public void setIntercept(double value)
```


يعيد أو يضبط النقطة التي يقطع فيها خط الاتجاه محور القيم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setInterceptAuto(boolean isInterceptAuto) {#setInterceptAuto-boolean-}
```
public void setInterceptAuto(boolean isInterceptAuto)
```


يضبط ما إذا كان Microsoft Workbook يحدد تلقائيًا تقاطع خط الاتجاه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isInterceptAuto | boolean |  |

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

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يعيد اسم خط الاتجاه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setNameAuto(boolean value) {#setNameAuto-boolean-}
```
public void setNameAuto(boolean value)
```


يعيد ما إذا كان Microsoft Excel يحدد تلقائيًا اسم خط الاتجاه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


يعيد أو يضبط ترتيب خط الاتجاه (عدد صحيح أكبر من 1) عندما يكون نوع خط الاتجاه متعدد الحدود. يجب أن يكون الترتيب بين 2 و 6.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPeriod(int value) {#setPeriod-int-}
```
public void setPeriod(int value)
```


يعيد أو يضبط الفترة لخط الاتجاه المتوسط المتحرك.

**Remarks**

يجب أن تكون هذه القيمة بين 2 و 255. ويجب أن تكون أقل من عدد نقاط المخطط في السلسلة

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

