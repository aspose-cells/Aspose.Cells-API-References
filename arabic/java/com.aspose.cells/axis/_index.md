---
title: "Axis"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على الكائن الذي يمثل محورًا في المخطط."
type: docs
url: /ar/java/com.aspose.cells/axis/
---

**Inheritance:**
java.lang.Object
```
public class Axis
```

يحتوي على الكائن الذي يمثل محورًا في المخطط.

**Example**

من الشفرات التالية، يمكنك تعلم كيفية تعيين الوحدة والقيمة القصوى والقيمة الدنيا للمحور.

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
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(4);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(20);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
         //Set the max value of value axis
         chart.getValueAxis().setMaxValue(200);
         //Set the min value of value axis
         chart.getValueAxis().setMinValue(0);
         //Set the major unit
         chart.getValueAxis().setMajorUnit(25);
         //Category(X) axis crosses at the maxinum value.
         chart.getValueAxis().setCrossType(CrossType.MAXIMUM);
         //Set he number of categories or series between tick-mark labels. 
         chart.getCategoryAxis().setTickLabelSpacing(2);
 
         //do your business
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | يحصل على [getArea()](../../com.aspose.cells/axis\#getArea--). |
| [getAxisBetweenCategories()](#getAxisBetweenCategories--) | يمثل ما إذا كان محور القيمة يعبر محور الفئة بين الفئات. |
| [getAxisLabels()](#getAxisLabels--) | يحصل على تسميات المحور بعد استدعاء طريقة Chart.Calculate(). |
| [getAxisLine()](#getAxisLine--) | يحصل على مظهر المحور. |
| [getAxisTexts()](#getAxisTexts--) | يحصل على تسميات المحور بعد استدعاء طريقة Chart.Calculate(). |
| [getBaseUnitScale()](#getBaseUnitScale--) | يمثل مقياس الوحدة الأساسية لمحور الفئة. |
| [getBins()](#getBins--) | يمثل الفواصل على محور المخطط (المدرج التكراري/باريتو). |
| [getCategoryType()](#getCategoryType--) | يمثل نوع محور الفئة. |
| [getClass()](#getClass--) |  |
| [getCrossAt()](#getCrossAt--) | يمثل النقطة على محور القيمة حيث يعبر محور الفئة ذلك. |
| [getCrossType()](#getCrossType--) | يمثل [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) على المحور المحدد حيث يعبر المحور الآخر. |
| [getCustUnit()](#getCustUnit--) | يحدد قيمة مخصصة لوحدة العرض. |
| [getCustomDisplayUnit()](#getCustomDisplayUnit--) | يحدد قيمة مخصصة لوحدة العرض. |
| [getCustomUnit()](#getCustomUnit--) | يحدد قيمة مخصصة لوحدة العرض. |
| [getDisplayUnit()](#getDisplayUnit--) | يمثل تسمية الوحدة للمحور المحدد. |
| [getDisplayUnitLabel()](#getDisplayUnitLabel--) | يمثل تسمية وحدة على محور في المخطط المحدد. |
| [getLogBase()](#getLogBase--) | يمثل القاعدة اللوغاريتمية. |
| [getMajorGridLines()](#getMajorGridLines--) | يمثل خطوط الشبكة الرئيسية على محور المخطط. |
| [getMajorTickMark()](#getMajorTickMark--) | يمثل نوع علامة الفاصل الكبرى للمحور المحدد. |
| [getMajorUnit()](#getMajorUnit--) | يمثل الوحدات الكبرى للمحور. |
| [getMajorUnitScale()](#getMajorUnitScale--) | يمثل مقياس الوحدة الكبرى لمحور الفئة. |
| [getMaxValue()](#getMaxValue--) | يمثل القيمة القصوى على محور القيم. |
| [getMinValue()](#getMinValue--) | يمثل القيمة الدنيا على محور القيم. |
| [getMinorGridLines()](#getMinorGridLines--) | يمثل خطوط الشبكة الصغرى على محور المخطط. |
| [getMinorTickMark()](#getMinorTickMark--) | يمثل نوع علامة الفاصل الصغرى للمحور المحدد. |
| [getMinorUnit()](#getMinorUnit--) | يمثل الوحدات الصغرى للمحور. |
| [getMinorUnitScale()](#getMinorUnitScale--) | يمثل مقياس الوحدة الكبرى لمحور الفئة. |
| [getTickLabelPosition()](#getTickLabelPosition--) | يمثل موضع تسميات علامات الفاصل على المحور المحدد. |
| [getTickLabelSpacing()](#getTickLabelSpacing--) | يمثل عدد الفئات أو السلاسل بين تسميات علامات الفاصل. |
| [getTickLabels()](#getTickLabels--) | يعيد كائن [getTickLabels()](../../com.aspose.cells/axis\\#getTickLabels--) الذي يمثل تسميات علامات الفاصل للمحور المحدد. |
| [getTickMarkSpacing()](#getTickMarkSpacing--) | يعيد أو يضبط عدد الفئات أو السلاسل بين علامات الفاصل. |
| [getTitle()](#getTitle--) | يحصل على عنوان هذا المحور في المخطط. |
| [hasMultiLevelLabels()](#hasMultiLevelLabels--) | يشير إلى ما إذا كانت التسميات ستظهر كمستوى متعدد. |
| [hashCode()](#hashCode--) |  |
| [isAutoTickLabelSpacing()](#isAutoTickLabelSpacing--) | يشير إلى ما إذا كان تباعد تسميات الفاصل تلقائيًا |
| [isAutomaticMajorUnit()](#isAutomaticMajorUnit--) | يشير إلى ما إذا كانت الوحدة الكبرى للمحور تُعيّن تلقائيًا. |
| [isAutomaticMaxValue()](#isAutomaticMaxValue--) | يشير إلى ما إذا كانت القيمة القصوى تُعيّن تلقائيًا. |
| [isAutomaticMinValue()](#isAutomaticMinValue--) | يشير إلى ما إذا كانت القيمة الدنيا تُعيّن تلقائيًا. |
| [isAutomaticMinorUnit()](#isAutomaticMinorUnit--) | يشير إلى ما إذا كانت الوحدة الصغرى للمحور تُعيّن تلقائيًا. |
| [isBaseUnitAuto()](#isBaseUnitAuto--) | يمثل ما إذا كانت الوحدة الأساسية تلقائية. |
| [isDisplayUnitLabelShown()](#isDisplayUnitLabelShown--) | يمثل ما إذا كان يتم عرض تسمية وحدة العرض على المحور المحدد. |
| [isLogarithmic()](#isLogarithmic--) | يمثل ما إذا كان نوع مقياس محور القيم لوغاريتميًا أم لا. |
| [isPlotOrderReversed()](#isPlotOrderReversed--) | يمثل ما إذا كان Microsoft Excel يرسم نقاط البيانات من الأخير إلى الأول. |
| [isVisible()](#isVisible--) | يمثل ما إذا كان المحور مرئيًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoTickLabelSpacing(boolean value)](#setAutoTickLabelSpacing-boolean-) | يشير إلى ما إذا كان تباعد تسميات الفاصل تلقائيًا |
| [setAutomaticMajorUnit(boolean value)](#setAutomaticMajorUnit-boolean-) | يشير إلى ما إذا كانت الوحدة الكبرى للمحور تُعيّن تلقائيًا. |
| [setAutomaticMaxValue(boolean value)](#setAutomaticMaxValue-boolean-) | يشير إلى ما إذا كانت القيمة القصوى تُعيّن تلقائيًا. |
| [setAutomaticMinValue(boolean value)](#setAutomaticMinValue-boolean-) | يشير إلى ما إذا كانت القيمة الدنيا تُعيّن تلقائيًا. |
| [setAutomaticMinorUnit(boolean value)](#setAutomaticMinorUnit-boolean-) | يشير إلى ما إذا كانت الوحدة الصغرى للمحور تُعيّن تلقائيًا. |
| [setAxisBetweenCategories(boolean value)](#setAxisBetweenCategories-boolean-) | يمثل ما إذا كان محور القيمة يعبر محور الفئة بين الفئات. |
| [setBaseUnitAuto(boolean value)](#setBaseUnitAuto-boolean-) | يمثل ما إذا كانت الوحدة الأساسية تلقائية. |
| [setBaseUnitScale(int value)](#setBaseUnitScale-int-) | يمثل مقياس الوحدة الأساسية لمحور الفئة. |
| [setCategoryType(int value)](#setCategoryType-int-) | يمثل نوع محور الفئة. |
| [setCrossAt(double value)](#setCrossAt-double-) | يمثل النقطة على محور القيمة حيث يعبر محور الفئة ذلك. |
| [setCrossType(int value)](#setCrossType-int-) | يمثل [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) على المحور المحدد حيث يعبر المحور الآخر. |
| [setCustUnit(int value)](#setCustUnit-int-) | يحدد قيمة مخصصة لوحدة العرض. |
| [setCustomDisplayUnit(double value)](#setCustomDisplayUnit-double-) | يحدد قيمة مخصصة لوحدة العرض. |
| [setCustomUnit(int value)](#setCustomUnit-int-) | يحدد قيمة مخصصة لوحدة العرض. |
| [setDisplayUnit(int value)](#setDisplayUnit-int-) | يمثل تسمية الوحدة للمحور المحدد. |
| [setDisplayUnitLabelShown(boolean value)](#setDisplayUnitLabelShown-boolean-) | يمثل ما إذا كان يتم عرض تسمية وحدة العرض على المحور المحدد. |
| [setHasMultiLevelLabels(boolean value)](#setHasMultiLevelLabels-boolean-) | يشير إلى ما إذا كانت التسميات ستظهر كمستوى متعدد. |
| [setLogBase(double value)](#setLogBase-double-) | يمثل القاعدة اللوغاريتمية. |
| [setLogarithmic(boolean value)](#setLogarithmic-boolean-) | يمثل ما إذا كان نوع مقياس محور القيم لوغاريتميًا أم لا. |
| [setMajorTickMark(int value)](#setMajorTickMark-int-) | يمثل نوع علامة الفاصل الكبرى للمحور المحدد. |
| [setMajorUnit(double value)](#setMajorUnit-double-) | يمثل الوحدات الكبرى للمحور. |
| [setMajorUnitScale(int value)](#setMajorUnitScale-int-) | يمثل مقياس الوحدة الكبرى لمحور الفئة. |
| [setMaxValue(Object value)](#setMaxValue-java.lang.Object-) | يمثل القيمة القصوى على محور القيم. |
| [setMinValue(Object value)](#setMinValue-java.lang.Object-) | يمثل القيمة الدنيا على محور القيم. |
| [setMinorTickMark(int value)](#setMinorTickMark-int-) | يمثل نوع علامة الفاصل الصغرى للمحور المحدد. |
| [setMinorUnit(double value)](#setMinorUnit-double-) | يمثل الوحدات الصغرى للمحور. |
| [setMinorUnitScale(int value)](#setMinorUnitScale-int-) | يمثل مقياس الوحدة الكبرى لمحور الفئة. |
| [setPlotOrderReversed(boolean value)](#setPlotOrderReversed-boolean-) | يمثل ما إذا كان Microsoft Excel يرسم نقاط البيانات من الأخير إلى الأول. |
| [setTickLabelPosition(int value)](#setTickLabelPosition-int-) | يمثل موضع تسميات علامات الفاصل على المحور المحدد. |
| [setTickLabelSpacing(int value)](#setTickLabelSpacing-int-) | يمثل عدد الفئات أو السلاسل بين تسميات علامات الفاصل. |
| [setTickMarkSpacing(int value)](#setTickMarkSpacing-int-) | يعيد أو يضبط عدد الفئات أو السلاسل بين علامات الفاصل. |
| [setVisible(boolean value)](#setVisible-boolean-) | يمثل ما إذا كان المحور مرئيًا. |
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
### getArea() {#getArea--}
```
public Area getArea()
```


يحصل على [getArea()](../../com.aspose.cells/axis\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAxisBetweenCategories() {#getAxisBetweenCategories--}
```
public boolean getAxisBetweenCategories()
```


يمثل ما إذا كان محور القيمة يعبر محور الفئة بين الفئات.

**Remarks**

تنطبق هذه الخاصية فقط على محاور الفئة، ولا تنطبق على المخططات ثلاثية الأبعاد.

**Returns:**
boolean
### getAxisLabels() {#getAxisLabels--}
```
public ArrayList getAxisLabels()
```


يحصل على تسميات المحور بعد استدعاء طريقة Chart.Calculate().

**Remarks**

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام طريقة Axis.GetAxisTexts. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ نوفمبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.util.ArrayList
### getAxisLine() {#getAxisLine--}
```
public Line getAxisLine()
```


يحصل على مظهر المحور.

**Returns:**
[Line](../../com.aspose.cells/line)
### getAxisTexts() {#getAxisTexts--}
```
public String[] getAxisTexts()
```


يحصل على تسميات المحور بعد استدعاء طريقة Chart.Calculate().

**Returns:**
java.lang.String[]
### getBaseUnitScale() {#getBaseUnitScale--}
```
public int getBaseUnitScale()
```


يمثل مقياس الوحدة الأساسية لمحور الفئة.

انظر [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

يأخذ تأثيره فقط عندما يتم تعيين خاصية CategoryType إلى TimeScale.

**Returns:**
int
### getBins() {#getBins--}
```
public AxisBins getBins()
```


يمثل الفواصل على محور المخطط (المدرج التكراري/باريتو).

**Remarks**

فقط لمخطط Histogram أو Pareto.

**Returns:**
[AxisBins](../../com.aspose.cells/axisbins)
### getCategoryType() {#getCategoryType--}
```
public int getCategoryType()
```


يمثل نوع محور الفئة.

انظر [CategoryType](../../com.aspose.cells/categorytype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCrossAt() {#getCrossAt--}
```
public double getCrossAt()
```


يمثل النقطة على محور القيمة حيث يعبر محور الفئة ذلك.

**Remarks**

يجب أن يكون الرقم عددًا صحيحًا عندما ينطبق على محور الفئة. ويجب أن تكون القيمة بين 1 و 31999.

**Returns:**
double
### getCrossType() {#getCrossType--}
```
public int getCrossType()
```


يمثل [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) على المحور المحدد حيث يعبر المحور الآخر.

انظر [CrossType](../../com.aspose.cells/crosstype).

**Returns:**
int
### getCustUnit() {#getCustUnit--}
```
public int getCustUnit()
```


يحدد قيمة مخصصة لوحدة العرض.

**Remarks**

ملاحظة: هذه الخاصية الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية Axis.CustomUnit. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getCustomDisplayUnit() {#getCustomDisplayUnit--}
```
public double getCustomDisplayUnit()
```


يحدد قيمة مخصصة لوحدة العرض.

**Returns:**
double
### getCustomUnit() {#getCustomUnit--}
```
public int getCustomUnit()
```


يحدد قيمة مخصصة لوحدة العرض.

**Remarks**

ملاحظة: هذه الخاصية الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية Axis.CustomDisplayUnit. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getDisplayUnit() {#getDisplayUnit--}
```
public int getDisplayUnit()
```


يمثل تسمية الوحدة للمحور المحدد.

انظر [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Returns:**
int
### getDisplayUnitLabel() {#getDisplayUnitLabel--}
```
public DisplayUnitLabel getDisplayUnitLabel()
```


يمثل تسمية وحدة على محور في المخطط المحدد. تسميات الوحدات مفيدة لتصوير القيم الكبيرة - على سبيل المثال، بالملايين أو المليارات.

**Returns:**
[DisplayUnitLabel](../../com.aspose.cells/displayunitlabel)
### getLogBase() {#getLogBase--}
```
public double getLogBase()
```


يمثل القاعدة اللوغاريتمية. القيمة الافتراضية هي 10.

**Returns:**
double
### getMajorGridLines() {#getMajorGridLines--}
```
public Line getMajorGridLines()
```


يمثل خطوط الشبكة الرئيسية على محور المخطط.

**Example**

```
         chart.getValueAxis().getMajorGridLines().setVisible(false);
         chart.getCategoryAxis().getMajorGridLines().setVisible(true);
```

**Returns:**
[Line](../../com.aspose.cells/line)
### getMajorTickMark() {#getMajorTickMark--}
```
public int getMajorTickMark()
```


يمثل نوع علامة الفاصل الكبرى للمحور المحدد.

انظر [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMajorUnit() {#getMajorUnit--}
```
public double getMajorUnit()
```


يمثل الوحدات الكبرى للمحور.

**Remarks**

يجب أن تكون الوحدات الرئيسية أكبر من الصفر.

**Returns:**
double
### getMajorUnitScale() {#getMajorUnitScale--}
```
public int getMajorUnitScale()
```


يمثل مقياس الوحدة الكبرى لمحور الفئة.

انظر [TimeUnit](../../com.aspose.cells/timeunit).

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         /*TimeUnit*/int majorUnitScale = chart.getCategoryAxis().getMajorUnitScale(); //get
         chart.getCategoryAxis().setMajorUnitScale(majorUnitScale); //set
         chart.getCategoryAxis().setMajorUnit(2);
```

**Returns:**
int
### getMaxValue() {#getMaxValue--}
```
public Object getMaxValue()
```


يمثل القيمة القصوى على محور القيم.

**Remarks**

يمكن أن يكون نوع maxValue فقط double أو DateTime

**Returns:**
java.lang.Object
### getMinValue() {#getMinValue--}
```
public Object getMinValue()
```


يمثل القيمة الدنيا على محور القيم.

**Remarks**

يمكن أن يكون نوع minValue فقط double أو DateTime

**Returns:**
java.lang.Object
### getMinorGridLines() {#getMinorGridLines--}
```
public Line getMinorGridLines()
```


يمثل خطوط الشبكة الصغرى على محور المخطط.

**Returns:**
[Line](../../com.aspose.cells/line)
### getMinorTickMark() {#getMinorTickMark--}
```
public int getMinorTickMark()
```


يمثل نوع علامة الفاصل الصغرى للمحور المحدد.

انظر [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMinorUnit() {#getMinorUnit--}
```
public double getMinorUnit()
```


يمثل الوحدات الصغرى للمحور.

**Remarks**

يجب أن تكون الوحدات الفرعية أكبر من الصفر.

**Returns:**
double
### getMinorUnitScale() {#getMinorUnitScale--}
```
public int getMinorUnitScale()
```


يمثل مقياس الوحدة الكبرى لمحور الفئة.

انظر [TimeUnit](../../com.aspose.cells/timeunit).

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         chart.getCategoryAxis().setMinorUnitScale(TimeUnit.MONTHS);
         chart.getCategoryAxis().setMinorUnit(2);
```

**Returns:**
int
### getTickLabelPosition() {#getTickLabelPosition--}
```
public int getTickLabelPosition()
```


يمثل موضع تسميات علامات الفاصل على المحور المحدد.

انظر [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Returns:**
int
### getTickLabelSpacing() {#getTickLabelSpacing--}
```
public int getTickLabelSpacing()
```


يمثل عدد الفئات أو السلاسل بين تسميات علامات الفواصل. ينطبق فقط على محاور الفئة والسلاسل.

**Remarks**

يجب أن يكون الرقم بين 1 و 31999.

**Returns:**
int
### getTickLabels() {#getTickLabels--}
```
public TickLabels getTickLabels()
```


يعيد كائن [getTickLabels()](../../com.aspose.cells/axis\\#getTickLabels--) الذي يمثل تسميات علامات الفاصل للمحور المحدد.

**Returns:**
[TickLabels](../../com.aspose.cells/ticklabels)
### getTickMarkSpacing() {#getTickMarkSpacing--}
```
public int getTickMarkSpacing()
```


يعيد أو يضبط عدد الفئات أو السلاسل بين علامات الفواصل. ينطبق فقط على محاور الفئة والسلاسل.

**Remarks**

يجب أن يكون الرقم بين 1 و 31999.

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


يحصل على عنوان هذا المحور في المخطط.

**Returns:**
[Title](../../com.aspose.cells/title)
### hasMultiLevelLabels() {#hasMultiLevelLabels--}
```
public boolean hasMultiLevelLabels()
```


يشير إلى ما إذا كانت التسميات ستظهر كمستوى متعدد.

**Remarks**

صالح فقط لمحور الفئة.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoTickLabelSpacing() {#isAutoTickLabelSpacing--}
```
public boolean isAutoTickLabelSpacing()
```


يشير إلى ما إذا كان تباعد تسميات الفاصل تلقائيًا

**Returns:**
boolean
### isAutomaticMajorUnit() {#isAutomaticMajorUnit--}
```
public boolean isAutomaticMajorUnit()
```


يشير إلى ما إذا كانت الوحدة الكبرى للمحور تُعيّن تلقائيًا.

**Returns:**
boolean
### isAutomaticMaxValue() {#isAutomaticMaxValue--}
```
public boolean isAutomaticMaxValue()
```


يشير إلى ما إذا كانت القيمة القصوى تُعيّن تلقائيًا.

**Returns:**
boolean
### isAutomaticMinValue() {#isAutomaticMinValue--}
```
public boolean isAutomaticMinValue()
```


يشير إلى ما إذا كانت القيمة الدنيا تُعيّن تلقائيًا.

**Returns:**
boolean
### isAutomaticMinorUnit() {#isAutomaticMinorUnit--}
```
public boolean isAutomaticMinorUnit()
```


يشير إلى ما إذا كانت الوحدة الصغرى للمحور تُعيّن تلقائيًا.

**Returns:**
boolean
### isBaseUnitAuto() {#isBaseUnitAuto--}
```
public boolean isBaseUnitAuto()
```


يمثل ما إذا كانت الوحدة الأساسية تلقائية.

**Returns:**
boolean
### isDisplayUnitLabelShown() {#isDisplayUnitLabelShown--}
```
public boolean isDisplayUnitLabelShown()
```


يمثل ما إذا كان يتم عرض تسمية وحدة العرض على المحور المحدد.

**Remarks**

القيمة الافتراضية هي True. يعمل فقط عندما لا تكون [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) هي [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE).

**Returns:**
boolean
### isLogarithmic() {#isLogarithmic--}
```
public boolean isLogarithmic()
```


يمثل ما إذا كان نوع مقياس محور القيم لوغاريتميًا أم لا.

**Returns:**
boolean
### isPlotOrderReversed() {#isPlotOrderReversed--}
```
public boolean isPlotOrderReversed()
```


يمثل ما إذا كان Microsoft Excel يرسم نقاط البيانات من الأخير إلى الأول.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


يمثل ما إذا كان المحور مرئيًا.

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




### setAutoTickLabelSpacing(boolean value) {#setAutoTickLabelSpacing-boolean-}
```
public void setAutoTickLabelSpacing(boolean value)
```


يشير إلى ما إذا كان تباعد تسميات الفاصل تلقائيًا

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutomaticMajorUnit(boolean value) {#setAutomaticMajorUnit-boolean-}
```
public void setAutomaticMajorUnit(boolean value)
```


يشير إلى ما إذا كانت الوحدة الكبرى للمحور تُعيّن تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutomaticMaxValue(boolean value) {#setAutomaticMaxValue-boolean-}
```
public void setAutomaticMaxValue(boolean value)
```


يشير إلى ما إذا كانت القيمة القصوى تُعيّن تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutomaticMinValue(boolean value) {#setAutomaticMinValue-boolean-}
```
public void setAutomaticMinValue(boolean value)
```


يشير إلى ما إذا كانت القيمة الدنيا تُعيّن تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutomaticMinorUnit(boolean value) {#setAutomaticMinorUnit-boolean-}
```
public void setAutomaticMinorUnit(boolean value)
```


يشير إلى ما إذا كانت الوحدة الصغرى للمحور تُعيّن تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAxisBetweenCategories(boolean value) {#setAxisBetweenCategories-boolean-}
```
public void setAxisBetweenCategories(boolean value)
```


يمثل ما إذا كان محور القيمة يعبر محور الفئة بين الفئات.

**Remarks**

تنطبق هذه الخاصية فقط على محاور الفئة، ولا تنطبق على المخططات ثلاثية الأبعاد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBaseUnitAuto(boolean value) {#setBaseUnitAuto-boolean-}
```
public void setBaseUnitAuto(boolean value)
```


يمثل ما إذا كانت الوحدة الأساسية تلقائية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBaseUnitScale(int value) {#setBaseUnitScale-int-}
```
public void setBaseUnitScale(int value)
```


يمثل مقياس الوحدة الأساسية لمحور الفئة.

انظر [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

يأخذ تأثيره فقط عندما يتم تعيين خاصية CategoryType إلى TimeScale.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCategoryType(int value) {#setCategoryType-int-}
```
public void setCategoryType(int value)
```


يمثل نوع محور الفئة.

انظر [CategoryType](../../com.aspose.cells/categorytype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCrossAt(double value) {#setCrossAt-double-}
```
public void setCrossAt(double value)
```


يمثل النقطة على محور القيمة حيث يعبر محور الفئة ذلك.

**Remarks**

يجب أن يكون الرقم عددًا صحيحًا عندما ينطبق على محور الفئة. ويجب أن تكون القيمة بين 1 و 31999.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setCrossType(int value) {#setCrossType-int-}
```
public void setCrossType(int value)
```


يمثل [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) على المحور المحدد حيث يعبر المحور الآخر.

انظر [CrossType](../../com.aspose.cells/crosstype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCustUnit(int value) {#setCustUnit-int-}
```
public void setCustUnit(int value)
```


يحدد قيمة مخصصة لوحدة العرض.

**Remarks**

ملاحظة: هذه الخاصية الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية Axis.CustomUnit. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCustomDisplayUnit(double value) {#setCustomDisplayUnit-double-}
```
public void setCustomDisplayUnit(double value)
```


يحدد قيمة مخصصة لوحدة العرض.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setCustomUnit(int value) {#setCustomUnit-int-}
```
public void setCustomUnit(int value)
```


يحدد قيمة مخصصة لوحدة العرض.

**Remarks**

ملاحظة: هذه الخاصية الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية Axis.CustomDisplayUnit. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDisplayUnit(int value) {#setDisplayUnit-int-}
```
public void setDisplayUnit(int value)
```


يمثل تسمية الوحدة للمحور المحدد.

انظر [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDisplayUnitLabelShown(boolean value) {#setDisplayUnitLabelShown-boolean-}
```
public void setDisplayUnitLabelShown(boolean value)
```


يمثل ما إذا كان يتم عرض تسمية وحدة العرض على المحور المحدد.

**Remarks**

القيمة الافتراضية هي True. يعمل فقط عندما لا تكون [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) هي [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasMultiLevelLabels(boolean value) {#setHasMultiLevelLabels-boolean-}
```
public void setHasMultiLevelLabels(boolean value)
```


يشير إلى ما إذا كانت التسميات ستظهر كمستوى متعدد.

**Remarks**

صالح فقط لمحور الفئة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLogBase(double value) {#setLogBase-double-}
```
public void setLogBase(double value)
```


يمثل القاعدة اللوغاريتمية. القيمة الافتراضية هي 10.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setLogarithmic(boolean value) {#setLogarithmic-boolean-}
```
public void setLogarithmic(boolean value)
```


يمثل ما إذا كان نوع مقياس محور القيم لوغاريتميًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setMajorTickMark(int value) {#setMajorTickMark-int-}
```
public void setMajorTickMark(int value)
```


يمثل نوع علامة الفاصل الكبرى للمحور المحدد.

انظر [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMajorUnit(double value) {#setMajorUnit-double-}
```
public void setMajorUnit(double value)
```


يمثل الوحدات الكبرى للمحور.

**Remarks**

يجب أن تكون الوحدات الرئيسية أكبر من الصفر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setMajorUnitScale(int value) {#setMajorUnitScale-int-}
```
public void setMajorUnitScale(int value)
```


يمثل مقياس الوحدة الكبرى لمحور الفئة.

انظر [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMaxValue(Object value) {#setMaxValue-java.lang.Object-}
```
public void setMaxValue(Object value)
```


يمثل القيمة القصوى على محور القيم.

**Remarks**

يمكن أن يكون نوع maxValue فقط double أو DateTime

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

### setMinValue(Object value) {#setMinValue-java.lang.Object-}
```
public void setMinValue(Object value)
```


يمثل القيمة الدنيا على محور القيم.

**Remarks**

يمكن أن يكون نوع minValue فقط double أو DateTime

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

### setMinorTickMark(int value) {#setMinorTickMark-int-}
```
public void setMinorTickMark(int value)
```


يمثل نوع علامة الفاصل الصغرى للمحور المحدد.

انظر [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMinorUnit(double value) {#setMinorUnit-double-}
```
public void setMinorUnit(double value)
```


يمثل الوحدات الصغرى للمحور.

**Remarks**

يجب أن تكون الوحدات الفرعية أكبر من الصفر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setMinorUnitScale(int value) {#setMinorUnitScale-int-}
```
public void setMinorUnitScale(int value)
```


يمثل مقياس الوحدة الكبرى لمحور الفئة.

انظر [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPlotOrderReversed(boolean value) {#setPlotOrderReversed-boolean-}
```
public void setPlotOrderReversed(boolean value)
```


يمثل ما إذا كان Microsoft Excel يرسم نقاط البيانات من الأخير إلى الأول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTickLabelPosition(int value) {#setTickLabelPosition-int-}
```
public void setTickLabelPosition(int value)
```


يمثل موضع تسميات علامات الفاصل على المحور المحدد.

انظر [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTickLabelSpacing(int value) {#setTickLabelSpacing-int-}
```
public void setTickLabelSpacing(int value)
```


يمثل عدد الفئات أو السلاسل بين تسميات علامات الفواصل. ينطبق فقط على محاور الفئة والسلاسل.

**Remarks**

يجب أن يكون الرقم بين 1 و 31999.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTickMarkSpacing(int value) {#setTickMarkSpacing-int-}
```
public void setTickMarkSpacing(int value)
```


يعيد أو يضبط عدد الفئات أو السلاسل بين علامات الفواصل. ينطبق فقط على محاور الفئة والسلاسل.

**Remarks**

يجب أن يكون الرقم بين 1 و 31999.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


يمثل ما إذا كان المحور مرئيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

