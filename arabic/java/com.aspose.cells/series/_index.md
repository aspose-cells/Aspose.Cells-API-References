---
title: "Series"
second_title: "Aspose.Cells for Java API Reference"
description: "يغلف الكائن الذي يمثل سلسلة بيانات واحدة في مخطط."
type: docs
url: /ar/java/com.aspose.cells/series/
---

**Inheritance:**
java.lang.Object
```
public class Series
```

يغلف الكائن الذي يمثل سلسلة بيانات واحدة في مخطط.

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
         int seriesIndex = chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         Series series = chart.getNSeries().get(seriesIndex);
         //Setting the values of the series.
         series.setValues("=B1:B4");
         //Changing the chart type of the series.
         series.setType(ChartType.LINE);
         //Setting marker properties.
         series.getMarker().setMarkerStyle(ChartMarkerType.CIRCLE);
         series.getMarker().setForegroundColorSetType(FormattingType.AUTOMATIC);
         series.getMarker().setForegroundColor(com.aspose.cells.Color.getBlack());
         series.getMarker().setBackgroundColorSetType(FormattingType.AUTOMATIC);
 
         //do your business
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | يمثل مساحة الخلفية لكائن Series. |
| [getBar3DShapeType()](#getBar3DShapeType--) | يحصل على نوع الشكل ثلاثي الأبعاد المستخدم مع مخطط العمود أو الشريط ثلاثي الأبعاد. |
| [getBorder()](#getBorder--) | يمثل حد كائن Series. |
| [getBubbleScale()](#getBubbleScale--) | يحصل على معامل المقياس للفقاعات في مجموعة المخطط المحددة. |
| [getBubbleSizeRepresents()](#getBubbleSizeRepresents--) | يحصل على ما تمثله حجم الفقعة في مخطط الفقاعات. |
| [getBubbleSizes()](#getBubbleSizes--) | يحصل على قيم حجم الفقاعات لسلسلة المخطط. |
| [getCachedCategoryValues()](#getCachedCategoryValues--) | يحصل على قيم الفئات المخزنة مؤقتًا للسلسلة |
| [getCachedValues()](#getCachedValues--) | يحصل على القيم المخزنة مؤقتًا للسلسلة |
| [getCategoryValues()](#getCategoryValues--) | يحصل على قيم الفئات الفعلية المستخدمة لرسم كل نقطة من هذه السلسلة في المخطط. |
| [getClass()](#getClass--) |  |
| [getCountOfDataValues()](#getCountOfDataValues--) | يحصل على عدد قيم البيانات. |
| [getDataLabels()](#getDataLabels--) | يمثل كائن DataLabels للسلسلة المحددة ASeries. |
| [getDisplayName()](#getDisplayName--) | يحصل على اسم السلسلة الذي يُعرض على رسم المخطط. |
| [getDoughnutHoleSize()](#getDoughnutHoleSize--) | يرجع أو يضبط حجم الفتحة في مجموعة مخطط الدونات. |
| [getDownBars()](#getDownBars--) | يرجع كائن [DropBars](../../com.aspose.cells/dropbars) يمثل الأشرطة السفلية في مخطط الخط. |
| [getDropLines()](#getDropLines--) | يرجع كائن [Line](../../com.aspose.cells/line) يمثل خطوط السقوط لسلسلة في مخطط الخط أو مخطط المنطقة. |
| [getExplosion()](#getExplosion--) | المسافة بين شريحة الفطيرة المفتوحة ومركز مخطط الفطيرة تُعبّر عنها كنسبة مئوية من قطر الفطيرة. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | يحصل على زاوية الشريحة الأولى من مخطط الفطيرة أو مخطط الدونات، بالدرجات (مع اتجاه عقارب الساعة من العمودي). |
| [getGapWidth()](#getGapWidth--) | يرجع أو يضبط المسافة بين مجموعات الأعمدة أو الأشرطة، كنسبة مئوية من عرض العمود أو الشريط. |
| [getHas3DEffect()](#getHas3DEffect--) | صحيح إذا كانت السلسلة ذات مظهر ثلاثي الأبعاد. |
| [getHiLoLines()](#getHiLoLines--) | يرجع كائن HiLoLines يمثل خطوط الارتفاع-الانخفاض لسلسلة في مخطط الخط. |
| [getLayoutProperties()](#getLayoutProperties--) | يمثل خصائص التخطيط. |
| [getLeaderLines()](#getLeaderLines--) | يمثل خطوط القائد في المخطط. |
| [getLegendEntry()](#getLegendEntry--) | يحصل على مدخل الأسطورة وفقًا لهذه السلسلة. |
| [getMarker()](#getMarker--) | يحصل على [getMarker()](../../com.aspose.cells/series\#getMarker--). |
| [getName()](#getName--) | يحصل على اسم سلسلة البيانات. |
| [getOverlap()](#getOverlap--) | يحدد كيفية تموضع الأشرطة والأعمدة. |
| [getPlotOnSecondAxis()](#getPlotOnSecondAxis--) | يشير إلى ما إذا كانت هذه السلسلة مرسومة على المحور القيمي الثاني. |
| [getPointValues()](#getPointValues--) | يحصل على القيم الفعلية المستخدمة لرسم كل نقطة من هذه السلسلة في المخطط. |
| [getPoints()](#getPoints--) | يحصل على مجموعة النقاط في سلسلة داخل مخطط. |
| [getSecondPlotSize()](#getSecondPlotSize--) | يعيد أو يضبط حجم القسم الثانوي إما في مخطط فطيرة داخل فطيرة أو شريط داخل فطيرة، كنسبة مئوية من حجم الفطيرة الأساسية. |
| [getSeriesLines()](#getSeriesLines--) | يعيد كائن SeriesLines الذي يمثل خطوط السلسلة لمخطط شريط مكدس أو مخطط عمود مكدس. |
| [getShadow()](#getShadow--) | صحيح إذا كانت السلسلة لها ظل. |
| [getShapeProperties()](#getShapeProperties--) | يحصل على كائن [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) الذي يحتوي على خصائص الشكل البصرية للسلسلة. |
| [getShowNegativeBubbles()](#getShowNegativeBubbles--) | صحيح إذا تم عرض الفقاعات السالبة لمجموعة المخطط. |
| [getSizeRepresents()](#getSizeRepresents--) | يحصل على ما تمثله حجم الفقعة في مخطط الفقاعات. |
| [getSmooth()](#getSmooth--) | يمثل تنعيم المنحنى. |
| [getSplitType()](#getSplitType--) | يعيد أو يضبط قيمة تحدد كيفية تحديد نقاط البيانات التي تكون في الفطيرة أو الشريط الثاني في مخطط فطيرة داخل فطيرة أو شريط داخل فطيرة. |
| [getSplitValue()](#getSplitValue--) | يعيد أو يضبط قيمة تُستخدم لتحديد نقاط البيانات التي تكون في الفطيرة أو الشريط الثاني في مخطط فطيرة داخل فطيرة أو شريط داخل فطيرة. |
| [getTrendLines()](#getTrendLines--) | يعيد جميع خطوط الاتجاه لهذه السلسلة. |
| [getType()](#getType--) | يحصل على نوع سلسلة البيانات. |
| [getUpBars()](#getUpBars--) | يعيد كائن DropBars الذي يمثل الأشرطة الصاعدة في مخطط خطي. |
| [getValues()](#getValues--) | يمثل قيم Y لهذه السلسلة في المخطط. |
| [getValuesFormatCode()](#getValuesFormatCode--) | يمثل رمز التنسيق لقائمة أرقام القيم. |
| [getXErrorBar()](#getXErrorBar--) | يمثل شريط الخطأ في الاتجاه X للسلسلة. |
| [getXValues()](#getXValues--) | يمثل قيم X لهذه السلسلة في المخطط. |
| [getXValuesFormatCode()](#getXValuesFormatCode--) | يمثل رمز التنسيق لقائمة أرقام قيم X. |
| [getYErrorBar()](#getYErrorBar--) | يمثل شريط الخطأ في الاتجاه Y للسلسلة. |
| [hasDropLines()](#hasDropLines--) | صحيح إذا كان المخطط يحتوي على خطوط إسقاط. |
| [hasHiLoLines()](#hasHiLoLines--) | صحيح إذا كان المخطط الخطي يحتوي على خطوط أعلى-أدنى. |
| [hasLeaderLines()](#hasLeaderLines--) | صحيح إذا كانت السلسلة لها خطوط ربط. |
| [hasRadarAxisLabels()](#hasRadarAxisLabels--) | صحيح إذا كان مخطط الرادار يحتوي على تسميات محور الفئات. |
| [hasSeriesLines()](#hasSeriesLines--) | صحيح إذا كان مخطط عمود مكدس أو مخطط شريط يحتوي على خطوط السلاسل أو إذا كان مخطط فطيرة داخل فطيرة أو مخطط شريط داخل فطيرة يحتوي على خطوط وصل بين القسمين. |
| [hasUpDownBars()](#hasUpDownBars--) | صحيح إذا كان مخطط خط يحتوي على أشرطة صعود وهبوط. |
| [hashCode()](#hashCode--) |  |
| [isAutoSplit()](#isAutoSplit--) | يشير إلى ما إذا كانت قيمة العتبة تلقائية. |
| [isColorVaried()](#isColorVaried--) | يمثل ما إذا كان لون النقاط متنوعًا. |
| [isFiltered()](#isFiltered--) | يشير إلى ما إذا كانت السلسلة محددة أو مفلترة. |
| [isVerticalValues()](#isVerticalValues--) | يشير إلى ما إذا كان مصدر البيانات عموديًا. |
| [move(int count)](#move-int-) | ينقل السلسلة للأعلى أو للأسفل. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBar3DShapeType(int value)](#setBar3DShapeType-int-) | يضبط نوع الشكل ثلاثي الأبعاد المستخدم مع مخطط الشريط أو العمود ثلاثي الأبعاد. |
| [setBubbleScale(int value)](#setBubbleScale-int-) | يضبط عامل المقياس للفقاعات في مجموعة المخطط المحددة. |
| [setBubbleSizeRepresents(int value)](#setBubbleSizeRepresents-int-) | يحصل على ما تمثله حجم الفقعة في مخطط الفقاعات. |
| [setBubbleSizes(String value)](#setBubbleSizes-java.lang.String-) | يضبط قيم حجم الفقاعات لسلسلة المخطط. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | يمثل ما إذا كان لون النقاط متنوعًا. |
| [setDoughnutHoleSize(int value)](#setDoughnutHoleSize-int-) | يرجع أو يضبط حجم الفتحة في مجموعة مخطط الدونات. |
| [setExplosion(int value)](#setExplosion-int-) | المسافة بين شريحة الفطيرة المفتوحة ومركز مخطط الفطيرة تُعبّر عنها كنسبة مئوية من قطر الفطيرة. |
| [setFiltered(boolean value)](#setFiltered-boolean-) | يشير إلى ما إذا كانت السلسلة محددة أو مفلترة. |
| [setFirstSliceAngle(short value)](#setFirstSliceAngle-short-) | يضبط زاوية الشريحة الأولى في مخطط الفطيرة أو مخطط الدونات، بالدرجات (عقارب الساعة من العمودي). |
| [setGapWidth(short value)](#setGapWidth-short-) | يرجع أو يضبط المسافة بين مجموعات الأعمدة أو الأشرطة، كنسبة مئوية من عرض العمود أو الشريط. |
| [setHas3DEffect(boolean value)](#setHas3DEffect-boolean-) | صحيح إذا كانت السلسلة ذات مظهر ثلاثي الأبعاد. |
| [setHasDropLines(boolean value)](#setHasDropLines-boolean-) | صحيح إذا كان المخطط يحتوي على خطوط إسقاط. |
| [setHasHiLoLines(boolean value)](#setHasHiLoLines-boolean-) | صحيح إذا كان المخطط الخطي يحتوي على خطوط أعلى-أدنى. |
| [setHasLeaderLines(boolean value)](#setHasLeaderLines-boolean-) | صحيح إذا كانت السلسلة لها خطوط ربط. |
| [setHasRadarAxisLabels(boolean value)](#setHasRadarAxisLabels-boolean-) | صحيح إذا كان مخطط الرادار يحتوي على تسميات محور الفئات. |
| [setHasSeriesLines(boolean value)](#setHasSeriesLines-boolean-) | صحيح إذا كان مخطط عمود مكدس أو مخطط شريط يحتوي على خطوط السلاسل أو إذا كان مخطط فطيرة داخل فطيرة أو مخطط شريط داخل فطيرة يحتوي على خطوط وصل بين القسمين. |
| [setHasUpDownBars(boolean value)](#setHasUpDownBars-boolean-) | صحيح إذا كان مخطط خط يحتوي على أشرطة صعود وهبوط. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم سلسلة البيانات. |
| [setOverlap(short value)](#setOverlap-short-) | يحدد كيفية تموضع الأشرطة والأعمدة. |
| [setPlotOnSecondAxis(boolean value)](#setPlotOnSecondAxis-boolean-) | يشير إلى ما إذا كانت هذه السلسلة مرسومة على المحور القيمي الثاني. |
| [setSecondPlotSize(short value)](#setSecondPlotSize-short-) | يعيد أو يضبط حجم القسم الثانوي إما في مخطط فطيرة داخل فطيرة أو شريط داخل فطيرة، كنسبة مئوية من حجم الفطيرة الأساسية. |
| [setShadow(boolean value)](#setShadow-boolean-) | صحيح إذا كانت السلسلة لها ظل. |
| [setShowNegativeBubbles(boolean value)](#setShowNegativeBubbles-boolean-) | صحيح إذا تم عرض الفقاعات السالبة لمجموعة المخطط. |
| [setSizeRepresents(int value)](#setSizeRepresents-int-) | يضبط ما يمثله حجم الفقاعة في مخطط الفقاعات. |
| [setSmooth(boolean value)](#setSmooth-boolean-) | يمثل تنعيم المنحنى. |
| [setSplitType(int value)](#setSplitType-int-) | يعيد أو يضبط قيمة تحدد كيفية تحديد نقاط البيانات التي تكون في الفطيرة أو الشريط الثاني في مخطط فطيرة داخل فطيرة أو شريط داخل فطيرة. |
| [setSplitValue(double value)](#setSplitValue-double-) | يعيد أو يضبط قيمة تُستخدم لتحديد نقاط البيانات التي تكون في الفطيرة أو الشريط الثاني في مخطط فطيرة داخل فطيرة أو شريط داخل فطيرة. |
| [setType(int value)](#setType-int-) | يضبط نوع سلسلة البيانات. |
| [setValues(String value)](#setValues-java.lang.String-) | يمثل قيم Y لهذه السلسلة في المخطط. |
| [setValuesFormatCode(String value)](#setValuesFormatCode-java.lang.String-) | يمثل رمز التنسيق لقائمة أرقام القيم. |
| [setXValues(String value)](#setXValues-java.lang.String-) | يمثل قيم X لهذه السلسلة في المخطط. |
| [setXValuesFormatCode(String value)](#setXValuesFormatCode-java.lang.String-) | يمثل رمز التنسيق لقائمة أرقام قيم X. |
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


يمثل مساحة الخلفية لكائن Series.

**Returns:**
[Area](../../com.aspose.cells/area)
### getBar3DShapeType() {#getBar3DShapeType--}
```
public int getBar3DShapeType()
```


يحصل على نوع الشكل ثلاثي الأبعاد المستخدم مع مخطط العمود أو الشريط ثلاثي الأبعاد.

انظر [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


يمثل حد كائن Series.

**Returns:**
[Line](../../com.aspose.cells/line)
### getBubbleScale() {#getBubbleScale--}
```
public int getBubbleScale()
```


يحصل على عامل المقياس للفقاعات في مجموعة المخطط المحددة. يمكن أن يكون قيمة عددية صحيحة من 0 (صفر) إلى 300، تمثل نسبة مئوية من الحجم الافتراضي. ينطبق فقط على مخططات الفقاعات.

**Returns:**
int
### getBubbleSizeRepresents() {#getBubbleSizeRepresents--}
```
public int getBubbleSizeRepresents()
```


يحصل على ما تمثله حجم الفقعة في مخطط الفقاعات.

انظر [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

ملاحظة: هذه العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام الخاصية Aspose.Cells.Charts.Series.SizeRepresents. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2012. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getBubbleSizes() {#getBubbleSizes--}
```
public String getBubbleSizes()
```


يحصل على قيم حجم الفقاعات لسلسلة المخطط.

**Remarks**

فقط لـ [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) أو [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Returns:**
java.lang.String
### getCachedCategoryValues() {#getCachedCategoryValues--}
```
public ArrayList getCachedCategoryValues()
```


يحصل على قيم الفئات المخزنة مؤقتًا للسلسلة

**Remarks**

ملاحظة: هذه الخاصية حاليًا للاستخدام الداخلي فقط. سيتم تعديلها أو إزالتها في الإصدار التالي.

**Returns:**
java.util.ArrayList
### getCachedValues() {#getCachedValues--}
```
public ArrayList getCachedValues()
```


يحصل على القيم المخزنة مؤقتًا للسلسلة

**Remarks**

ملاحظة: هذه الخاصية حاليًا للاستخدام الداخلي فقط. سيتم تعديلها أو إزالتها في الإصدار التالي.

**Returns:**
java.util.ArrayList
### getCategoryValues() {#getCategoryValues--}
```
public ChartDataValue[][] getCategoryValues()
```


يحصل على قيم الفئات الفعلية المستخدمة لرسم كل نقطة من هذه السلسلة في المخطط.

**Remarks**

توفر هذه الخاصية طريقة مريحة واحدة للحصول على القيم الفعلية المقابلة للبيانات المعرفة بواسطة [getXValues()](../../com.aspose.cells/series\#getXValues--)، خاصة عندما يكون مصدر البيانات المحدد رابطًا خارجيًا أو صيغة، ... إلخ.

**Example**

```
         //Standalone example
         Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Chart chart = worksheet.getCharts().get(0);
         chart.calculate();
         String XValues = chart.getNSeries().get(0).getXValues();
         // XValues may be like "[External.xlsx]Sheet1!$B$2:$C$6" which is complicated
         // for user to get the actual values(the values may be linked to another workbook,
         // or cached in current workbook). Here you can use CategoryValues property
         // to get the category values actually displayed in the Excel interface
         // in the form of a two-dimensional array.
         ChartDataValue[][] v1 = chart.getNSeries().get(0).getCategoryValues();
```

**Returns:**
com.aspose.cells.ChartDataValue[][]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCountOfDataValues() {#getCountOfDataValues--}
```
public int getCountOfDataValues()
```


يحصل على عدد قيم البيانات.

**Returns:**
int
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


يمثل كائن DataLabels للسلسلة المحددة ASeries.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


يحصل على اسم السلسلة الذي يُعرض على رسم المخطط.

**Returns:**
java.lang.String
### getDoughnutHoleSize() {#getDoughnutHoleSize--}
```
public int getDoughnutHoleSize()
```


يعيد أو يضبط حجم الفتحة في مجموعة مخطط الدونات. يُعبّر عن حجم الفتحة كنسبة مئوية من حجم المخطط، بين 10 و 90 بالمائة.

**Returns:**
int
### getDownBars() {#getDownBars--}
```
public DropBars getDownBars()
```


يعيد كائنًا من نوع [DropBars](../../com.aspose.cells/dropbars) يمثل الأشرطة السفلية في مخطط خط. ينطبق فقط على مخططات الخط.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getDropLines() {#getDropLines--}
```
public Line getDropLines()
```


يعيد كائنًا من نوع [Line](../../com.aspose.cells/line) يمثل خطوط الإسقاط لسلسلة في مخطط الخط أو مخطط المنطقة. ينطبق فقط على مخططات الخط أو مخططات المنطقة.

**Returns:**
[Line](../../com.aspose.cells/line)
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


المسافة بين شريحة الفطيرة المفتوحة ومركز مخطط الفطيرة تُعبّر عنها كنسبة مئوية من قطر الفطيرة.

**Returns:**
int
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public short getFirstSliceAngle()
```


يحصل على زاوية الشريحة الأولى في مخطط الفطيرة أو مخطط الدونات، بالدرجات (مع اتجاه عقارب الساعة من العمودي). ينطبق فقط على مخططات الفطيرة، الفطيرة ثلاثية الأبعاد، والدونات، بقيم من 0 إلى 360.

**Returns:**
short
### getGapWidth() {#getGapWidth--}
```
public short getGapWidth()
```


يعيد أو يضبط المسافة بين مجموعات الأعمدة أو الأعمدة، كنسبة مئوية من عرض العمود أو الشريط. يجب أن تكون قيمة هذه الخاصية بين 0 و 500.

**Returns:**
short
### getHas3DEffect() {#getHas3DEffect--}
```
public boolean getHas3DEffect()
```


صحيح إذا كانت السلسلة ذات مظهر ثلاثي الأبعاد.

**Remarks**

ينطبق فقط على مخططات [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) أو [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Returns:**
boolean
### getHiLoLines() {#getHiLoLines--}
```
public Line getHiLoLines()
```


يرجع كائن HiLoLines الذي يمثل خطوط الارتفاع-الانخفاض لسلسلة في مخطط خطي. ينطبق فقط على المخططات الخطية.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLayoutProperties() {#getLayoutProperties--}
```
public SeriesLayoutProperties getLayoutProperties()
```


يمثل خصائص التخطيط.

**Returns:**
[SeriesLayoutProperties](../../com.aspose.cells/serieslayoutproperties)
### getLeaderLines() {#getLeaderLines--}
```
public Line getLeaderLines()
```


يمثل خطوط القائد في المخطط. خطوط القائد تربط تسميات البيانات بنقاط البيانات. هذا الكائن ليس مجموعة؛ لا يوجد كائن يمثل خط قائد واحد.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


يحصل على مدخل الأسطورة وفقًا لهذه السلسلة.

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


يحصل على [getMarker()](../../com.aspose.cells/series\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم سلسلة البيانات.

**Example**

```
         //Reference name to a cell
         chart.getNSeries().get(0).setName("=A1");
 
         //Set a string to name
         chart.getNSeries().get(0).setName("First Series");
```

**Returns:**
java.lang.String
### getOverlap() {#getOverlap--}
```
public short getOverlap()
```


يحدد كيفية تموضع الأشرطة والأعمدة. يمكن أن تكون قيمة بين -100 و 100. ينطبق فقط على مخططات الأشرطة ثنائية الأبعاد ومخططات الأعمدة ثنائية الأبعاد.

**Returns:**
short
### getPlotOnSecondAxis() {#getPlotOnSecondAxis--}
```
public boolean getPlotOnSecondAxis()
```


يشير إلى ما إذا كانت هذه السلسلة مرسومة على المحور القيمي الثاني.

**Returns:**
boolean
### getPointValues() {#getPointValues--}
```
public ChartDataValue[] getPointValues()
```


يحصل على القيم الفعلية المستخدمة لرسم كل نقطة من هذه السلسلة في المخطط.

**Remarks**

توفر هذه الخاصية طريقة مريحة للحصول على القيم الفعلية المقابلة للبيانات المعرفة بواسطة [getValues()](../../com.aspose.cells/series\#getValues--)، خاصة عندما يكون مصدر البيانات المحدد رابطًا خارجيًا أو صيغةً، ...إلخ.

**Example**

```
         Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Chart chart = worksheet.getCharts().get(0);
         chart.calculate();
         String Values = chart.getNSeries().get(0).getValues();
         // Values could be like "[External.xlsx]Sheet1!$A$1:$A$6" which is complicated
         // for user to get the actual values(the values may be linked to another workbook,
         // or cached in current workbook). Here you can use PointValues property
         // to get the values actually displayed in the Excel interface
         // in the form of an array.
         ChartDataValue[] v1 = chart.getNSeries().get(0).getPointValues();
```

**Returns:**
com.aspose.cells.ChartDataValue[]
### getPoints() {#getPoints--}
```
public ChartPointCollection getPoints()
```


يحصل على مجموعة النقاط في سلسلة داخل مخطط.

**Remarks**

عندما يكون المخطط Pie of Pie أو Bar of Pie، تكون النقطة الأخيرة هي نقطة أخرى في المخطط الدائري الأول.

**Returns:**
[ChartPointCollection](../../com.aspose.cells/chartpointcollection)
### getSecondPlotSize() {#getSecondPlotSize--}
```
public short getSecondPlotSize()
```


يرجع أو يحدد حجم القسم الثانوي إما في مخطط Pie of Pie أو مخطط Bar of Pie، كنسبة مئوية من حجم الدائرة الأساسية. يمكن أن تكون قيمة من 5 إلى 200.

**Returns:**
short
### getSeriesLines() {#getSeriesLines--}
```
public Line getSeriesLines()
```


يرجع كائن SeriesLines الذي يمثل خطوط السلسلة لمخطط شريط مكدس أو مخطط عمود مكدس. ينطبق فقط على مخططات الشريط المكدس والعمود المكدس.

**Returns:**
[Line](../../com.aspose.cells/line)
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


صحيح إذا كانت السلسلة لها ظل.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


يحصل على كائن [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) الذي يحتوي على خصائص الشكل البصرية للسلسلة.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShowNegativeBubbles() {#getShowNegativeBubbles--}
```
public boolean getShowNegativeBubbles()
```


صحيح إذا تم عرض الفقاعات السلبية لمجموعة المخطط. صالح فقط لمخططات الفقاعات.

**Returns:**
boolean
### getSizeRepresents() {#getSizeRepresents--}
```
public int getSizeRepresents()
```


يحصل على ما تمثله حجم الفقعة في مخطط الفقاعات.

انظر [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea يعني أن القيمة [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) هي مساحة الفقاعة. BubbleSizeRepresents.SizeIsWidth يعني أن القيمة [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) هي عرض الفقاعة.

**Returns:**
int
### getSmooth() {#getSmooth--}
```
public boolean getSmooth()
```


يمثل تنعيم المنحنى. صحيح إذا تم تشغيل تنعيم المنحنى لمخطط خطي أو مخطط مبعثر. ينطبق فقط على المخططات الخطية ومخططات المبعثر ذات الخطوط.

**Returns:**
boolean
### getSplitType() {#getSplitType--}
```
public int getSplitType()
```


يعيد أو يضبط قيمة تحدد كيفية تحديد نقاط البيانات التي تكون في الفطيرة أو الشريط الثاني في مخطط فطيرة داخل فطيرة أو شريط داخل فطيرة.

انظر إلى [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Returns:**
int
### getSplitValue() {#getSplitValue--}
```
public double getSplitValue()
```


يعيد أو يضبط قيمة تُستخدم لتحديد نقاط البيانات التي تكون في الفطيرة أو الشريط الثاني في مخطط فطيرة داخل فطيرة أو شريط داخل فطيرة.

**Returns:**
double
### getTrendLines() {#getTrendLines--}
```
public TrendlineCollection getTrendLines()
```


يعيد جميع خطوط الاتجاه لهذه السلسلة.

**Returns:**
[TrendlineCollection](../../com.aspose.cells/trendlinecollection)
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع سلسلة البيانات.

انظر إلى [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getUpBars() {#getUpBars--}
```
public DropBars getUpBars()
```


يرجع كائن DropBars الذي يمثل الأشرطة العلوية في مخطط خطي. ينطبق فقط على المخططات الخطية.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getValues() {#getValues--}
```
public String getValues()
```


يمثل قيم Y لهذه السلسلة في المخطط.

**Remarks**

للحصول على القيم الفعلية (المقابلة لكل نقطة في هذه السلسلة) المعرفة بواسطة هذه الخاصية، يرجى استخدام [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Returns:**
java.lang.String
### getValuesFormatCode() {#getValuesFormatCode--}
```
public String getValuesFormatCode()
```


يمثل رمز التنسيق لقائمة أرقام القيم.

**Returns:**
java.lang.String
### getXErrorBar() {#getXErrorBar--}
```
public ErrorBar getXErrorBar()
```


يمثل شريط الخطأ في الاتجاه X للسلسلة.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### getXValues() {#getXValues--}
```
public String getXValues()
```


يمثل قيم X لهذه السلسلة في المخطط.

**Remarks**

فقط لمخطط Scatter ومخطط Bubble. يرجى استخدام [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) لأنواع المخططات الأخرى. يُستخدم [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) للحصول على القيم الفئوية الفعلية لهذه السلسلة.

**Returns:**
java.lang.String
### getXValuesFormatCode() {#getXValuesFormatCode--}
```
public String getXValuesFormatCode()
```


يمثل رمز التنسيق لقائمة أرقام قيم X.

**Returns:**
java.lang.String
### getYErrorBar() {#getYErrorBar--}
```
public ErrorBar getYErrorBar()
```


يمثل شريط الخطأ في الاتجاه Y للسلسلة.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### hasDropLines() {#hasDropLines--}
```
public boolean hasDropLines()
```


صحيح إذا كان المخطط يحتوي على خطوط إسقاط. ينطبق فقط على المخطط الخطي أو مخططات المنطقة.

**Returns:**
boolean
### hasHiLoLines() {#hasHiLoLines--}
```
public boolean hasHiLoLines()
```


صحيح إذا كان المخطط الخطي يحتوي على خطوط الارتفاع-الانخفاض. ينطبق فقط على المخططات الخطية.

**Returns:**
boolean
### hasLeaderLines() {#hasLeaderLines--}
```
public boolean hasLeaderLines()
```


صحيح إذا كانت السلسلة لها خطوط ربط.

**Returns:**
boolean
### hasRadarAxisLabels() {#hasRadarAxisLabels--}
```
public boolean hasRadarAxisLabels()
```


صحيح إذا كان مخطط الرادار يحتوي على تسميات محور الفئة. ينطبق فقط على مخططات الرادار.

**Returns:**
boolean
### hasSeriesLines() {#hasSeriesLines--}
```
public boolean hasSeriesLines()
```


صحيح إذا كان مخطط العمود المكدس أو مخطط الشريط يحتوي على خطوط السلسلة أو إذا كان مخطط Pie of Pie أو مخطط Bar of Pie يحتوي على خطوط وصل بين القسمين. ينطبق فقط على مخططات العمود المكدس، ومخططات الشريط، ومخططات Pie of Pie، أو مخططات Bar of Pie.

**Returns:**
boolean
### hasUpDownBars() {#hasUpDownBars--}
```
public boolean hasUpDownBars()
```


صحيح إذا كان المخطط الخطي يحتوي على أشرطة صعود وهبوط. ينطبق فقط على المخططات الخطية.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSplit() {#isAutoSplit--}
```
public boolean isAutoSplit()
```


يشير إلى ما إذا كانت قيمة العتبة تلقائية.

**Returns:**
boolean
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


يمثل ما إذا كان لون النقاط متنوعًا. يجب أن يحتوي المخطط على سلسلة واحدة فقط أو أن يكون مخططًا دائريًا.

**Returns:**
boolean
### isFiltered() {#isFiltered--}
```
public boolean isFiltered()
```


يشير إلى ما إذا كانت السلسلة مختارة أو مفلترة. صحيح يعني أن هذه السلسلة مفلترة، ولن يتم عرضها على المخطط.

**Returns:**
boolean
### isVerticalValues() {#isVerticalValues--}
```
public boolean isVerticalValues()
```


يشير إلى ما إذا كان مصدر البيانات عموديًا.

**Returns:**
boolean
### move(int count) {#move-int-}
```
public void move(int count)
```


ينقل السلسلة للأعلى أو للأسفل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| العدد | int | عدد التحركات صعودًا أو هبوطًا. حرك السلسلة صعودًا إذا كانت هذه القيمة أقل من الصفر؛ حرك السلسلة هبوطًا إذا كانت هذه القيمة أكبر من الصفر. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBar3DShapeType(int value) {#setBar3DShapeType-int-}
```
public void setBar3DShapeType(int value)
```


يضبط نوع الشكل ثلاثي الأبعاد المستخدم مع مخطط الشريط أو العمود ثلاثي الأبعاد.

انظر [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBubbleScale(int value) {#setBubbleScale-int-}
```
public void setBubbleScale(int value)
```


يضبط معامل المقياس للفقاعات في مجموعة المخطط المحددة. يمكن أن تكون قيمة صحيحة من 0 (صفر) إلى 300، تمثل نسبة مئوية من الحجم الافتراضي. ينطبق فقط على مخططات الفقاعات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBubbleSizeRepresents(int value) {#setBubbleSizeRepresents-int-}
```
public void setBubbleSizeRepresents(int value)
```


يحصل على ما تمثله حجم الفقعة في مخطط الفقاعات.

انظر [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

ملاحظة: هذه العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام الخاصية Aspose.Cells.Charts.Series.SizeRepresents. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2012. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBubbleSizes(String value) {#setBubbleSizes-java.lang.String-}
```
public void setBubbleSizes(String value)
```


يضبط قيم حجم الفقاعات لسلسلة المخطط.

**Remarks**

فقط لـ [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) أو [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


يمثل ما إذا كان لون النقاط متنوعًا. يجب أن يحتوي المخطط على سلسلة واحدة فقط أو أن يكون مخططًا دائريًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDoughnutHoleSize(int value) {#setDoughnutHoleSize-int-}
```
public void setDoughnutHoleSize(int value)
```


يعيد أو يضبط حجم الفتحة في مجموعة مخطط الدونات. يُعبّر عن حجم الفتحة كنسبة مئوية من حجم المخطط، بين 10 و 90 بالمائة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```


المسافة بين شريحة الفطيرة المفتوحة ومركز مخطط الفطيرة تُعبّر عنها كنسبة مئوية من قطر الفطيرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setFiltered(boolean value) {#setFiltered-boolean-}
```
public void setFiltered(boolean value)
```


يشير إلى ما إذا كانت السلسلة مختارة أو مفلترة. صحيح يعني أن هذه السلسلة مفلترة، ولن يتم عرضها على المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFirstSliceAngle(short value) {#setFirstSliceAngle-short-}
```
public void setFirstSliceAngle(short value)
```


يضبط زاوية الشريحة الأولى في مخطط الفطيرة أو مخطط الدونات، بالدرجات (مع اتجاه عقارب الساعة من العمودي). ينطبق فقط على مخططات الفطيرة، الفطيرة ثلاثية الأبعاد، ومخططات الدونات، بقيم من 0 إلى 360.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | short |  |

### setGapWidth(short value) {#setGapWidth-short-}
```
public void setGapWidth(short value)
```


يعيد أو يضبط المسافة بين مجموعات الأعمدة أو الأعمدة، كنسبة مئوية من عرض العمود أو الشريط. يجب أن تكون قيمة هذه الخاصية بين 0 و 500.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | short |  |

### setHas3DEffect(boolean value) {#setHas3DEffect-boolean-}
```
public void setHas3DEffect(boolean value)
```


صحيح إذا كانت السلسلة ذات مظهر ثلاثي الأبعاد.

**Remarks**

ينطبق فقط على مخططات [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) أو [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasDropLines(boolean value) {#setHasDropLines-boolean-}
```
public void setHasDropLines(boolean value)
```


صحيح إذا كان المخطط يحتوي على خطوط إسقاط. ينطبق فقط على المخطط الخطي أو مخططات المنطقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasHiLoLines(boolean value) {#setHasHiLoLines-boolean-}
```
public void setHasHiLoLines(boolean value)
```


صحيح إذا كان المخطط الخطي يحتوي على خطوط الارتفاع-الانخفاض. ينطبق فقط على المخططات الخطية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasLeaderLines(boolean value) {#setHasLeaderLines-boolean-}
```
public void setHasLeaderLines(boolean value)
```


صحيح إذا كانت السلسلة لها خطوط ربط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasRadarAxisLabels(boolean value) {#setHasRadarAxisLabels-boolean-}
```
public void setHasRadarAxisLabels(boolean value)
```


صحيح إذا كان مخطط الرادار يحتوي على تسميات محور الفئة. ينطبق فقط على مخططات الرادار.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasSeriesLines(boolean value) {#setHasSeriesLines-boolean-}
```
public void setHasSeriesLines(boolean value)
```


صحيح إذا كان مخطط العمود المكدس أو مخطط الشريط يحتوي على خطوط السلسلة أو إذا كان مخطط Pie of Pie أو مخطط Bar of Pie يحتوي على خطوط وصل بين القسمين. ينطبق فقط على مخططات العمود المكدس، ومخططات الشريط، ومخططات Pie of Pie، أو مخططات Bar of Pie.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasUpDownBars(boolean value) {#setHasUpDownBars-boolean-}
```
public void setHasUpDownBars(boolean value)
```


صحيح إذا كان المخطط الخطي يحتوي على أشرطة صعود وهبوط. ينطبق فقط على المخططات الخطية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يضبط اسم سلسلة البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOverlap(short value) {#setOverlap-short-}
```
public void setOverlap(short value)
```


يحدد كيفية تموضع الأشرطة والأعمدة. يمكن أن تكون قيمة بين -100 و 100. ينطبق فقط على مخططات الأشرطة ثنائية الأبعاد ومخططات الأعمدة ثنائية الأبعاد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | short |  |

### setPlotOnSecondAxis(boolean value) {#setPlotOnSecondAxis-boolean-}
```
public void setPlotOnSecondAxis(boolean value)
```


يشير إلى ما إذا كانت هذه السلسلة مرسومة على المحور القيمي الثاني.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSecondPlotSize(short value) {#setSecondPlotSize-short-}
```
public void setSecondPlotSize(short value)
```


يرجع أو يحدد حجم القسم الثانوي إما في مخطط Pie of Pie أو مخطط Bar of Pie، كنسبة مئوية من حجم الدائرة الأساسية. يمكن أن تكون قيمة من 5 إلى 200.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | short |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


صحيح إذا كانت السلسلة لها ظل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowNegativeBubbles(boolean value) {#setShowNegativeBubbles-boolean-}
```
public void setShowNegativeBubbles(boolean value)
```


صحيح إذا تم عرض الفقاعات السلبية لمجموعة المخطط. صالح فقط لمخططات الفقاعات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSizeRepresents(int value) {#setSizeRepresents-int-}
```
public void setSizeRepresents(int value)
```


يضبط ما يمثله حجم الفقاعة في مخطط الفقاعات.

انظر [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea يعني أن القيمة [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) هي مساحة الفقاعة. BubbleSizeRepresents.SizeIsWidth يعني أن القيمة [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) هي عرض الفقاعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSmooth(boolean value) {#setSmooth-boolean-}
```
public void setSmooth(boolean value)
```


يمثل تنعيم المنحنى. صحيح إذا تم تشغيل تنعيم المنحنى لمخطط خطي أو مخطط مبعثر. ينطبق فقط على المخططات الخطية ومخططات المبعثر ذات الخطوط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSplitType(int value) {#setSplitType-int-}
```
public void setSplitType(int value)
```


يعيد أو يضبط قيمة تحدد كيفية تحديد نقاط البيانات التي تكون في الفطيرة أو الشريط الثاني في مخطط فطيرة داخل فطيرة أو شريط داخل فطيرة.

انظر إلى [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSplitValue(double value) {#setSplitValue-double-}
```
public void setSplitValue(double value)
```


يعيد أو يضبط قيمة تُستخدم لتحديد نقاط البيانات التي تكون في الفطيرة أو الشريط الثاني في مخطط فطيرة داخل فطيرة أو شريط داخل فطيرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


يضبط نوع سلسلة البيانات.

انظر إلى [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setValues(String value) {#setValues-java.lang.String-}
```
public void setValues(String value)
```


يمثل قيم Y لهذه السلسلة في المخطط.

**Remarks**

للحصول على القيم الفعلية (المقابلة لكل نقطة في هذه السلسلة) المعرفة بواسطة هذه الخاصية، يرجى استخدام [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setValuesFormatCode(String value) {#setValuesFormatCode-java.lang.String-}
```
public void setValuesFormatCode(String value)
```


يمثل رمز التنسيق لقائمة أرقام القيم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setXValues(String value) {#setXValues-java.lang.String-}
```
public void setXValues(String value)
```


يمثل قيم X لهذه السلسلة في المخطط.

**Remarks**

فقط لمخطط Scatter ومخطط Bubble. يرجى استخدام [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) لأنواع المخططات الأخرى. يُستخدم [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) للحصول على القيم الفئوية الفعلية لهذه السلسلة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setXValuesFormatCode(String value) {#setXValuesFormatCode-java.lang.String-}
```
public void setXValuesFormatCode(String value)
```


يمثل رمز التنسيق لقائمة أرقام قيم X.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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

