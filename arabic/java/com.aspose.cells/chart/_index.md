---
title: "مخطط"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على الكائن الذي يمثل مخطط Excel واحد."
type: docs
url: /ar/java/com.aspose.cells/chart/
---

**Inheritance:**
java.lang.Object
```
public class Chart
```

يحتوي على الكائن الذي يمثل مخطط Excel واحد.

**Example**

تظهر الشفرات التالية كيفية إنشاء مخطط باستخدام شفرات .NET.

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
 
         	int chartIndex = sheet.getCharts().add(ChartType.COLUMN, 9, 9, 21, 15);
 
         	Chart chart = sheet.getCharts().get(chartIndex);
         chart.setChartDataRange("A1:B4", true);
         	chart.setShowLegend(true);
         	chart.getTitle().setText("Income Analysis");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [calculate()](#calculate--) | يحسب المواضع المخصصة لمنطقة الرسم والمحاور إذا تم تعيين مواضعها تلقائيًا. |
| [calculate(ChartCalculateOptions calculateOptions)](#calculate-com.aspose.cells.ChartCalculateOptions-) | يحسب الموضع المخصص لمنطقة الرسم والمحاور إذا تم تعيين موضعها تلقائيًا، باستخدام خيارات حساب المخطط. |
| [changeTemplate(byte[] data)](#changeTemplate-byte---) | تغيير نوع المخطط باستخدام قالب مسبق. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActualChartSize()](#getActualChartSize--) | يحصل على الحجم الفعلي للمخطط بوحدة البكسل. |
| [getActualSize()](#getActualSize--) | يحصل على الحجم الفعلي للمخطط بوحدة البكسل. |
| [getAutoScaling()](#getAutoScaling--) | صحيح إذا كان Microsoft Excel يضبط مخططًا ثلاثي الأبعاد بحيث يكون حجمه أقرب إلى المخطط الثنائي الأبعاد المكافئ. |
| [getBackWall()](#getBackWall--) | يعيد كائنًا [getWalls()](../../com.aspose.cells/chart\\#getWalls--) يمثل الجدار الخلفي لمخطط ثلاثي الأبعاد. |
| [getCategoryAxis()](#getCategoryAxis--) | يحصل على المحور X للمخطط. |
| [getChartArea()](#getChartArea--) | يحصل على مساحة المخطط في ورقة العمل. |
| [getChartDataRange()](#getChartDataRange--) | يحصل على نطاق مصدر البيانات للمخطط. |
| [getChartDataTable()](#getChartDataTable--) | يمثل جدول بيانات المخطط. |
| [getChartObject()](#getChartObject--) | يمثل شكل المخطط؛ |
| [getChartShape()](#getChartShape--) | يمثل شكل المخطط؛ |
| [getClass()](#getClass--) |  |
| [getDepthPercent()](#getDepthPercent--) | يمثل عمق المخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 20 و2000 بالمئة). |
| [getDisplayNaAsBlank()](#getDisplayNaAsBlank--) | يشير إلى ما إذا كان يجب عرض \#N/A كقيمة فارغة. |
| [getElevation()](#getElevation--) | يمثل ارتفاع عرض المخطط ثلاثي الأبعاد، بالدرجات. |
| [getFilteredNSeries()](#getFilteredNSeries--) | يحصل على مجموعة [SeriesCollection](../../com.aspose.cells/seriescollection) التي تمثل سلسلة البيانات التي تم تصفيتها في المخطط. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | يحصل على زاوية الشريحة الأولى من مخطط الفطيرة أو مخطط الدونات، بالدرجات (مع اتجاه عقارب الساعة من العمودي). |
| [getFloor()](#getFloor--) | يرجع كائن [getFloor()](../../com.aspose.cells/chart\#getFloor--) الذي يمثل جدران المخطط ثلاثي الأبعاد. |
| [getGapDepth()](#getGapDepth--) | يحصل على المسافة بين سلاسل البيانات في مخطط ثلاثي الأبعاد، كنسبة مئوية من عرض العلامة. |
| [getGapWidth()](#getGapWidth--) | يرجع أو يضبط المسافة بين مجموعات الأعمدة أو الأشرطة، كنسبة مئوية من عرض العمود أو الشريط. |
| [getHeightPercent()](#getHeightPercent--) | يرجع أو يضبط ارتفاع المخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 5 و500 بالمئة). |
| [getHidePivotFieldButtons()](#getHidePivotFieldButtons--) | يشير إلى ما إذا كان يجب إخفاء أزرار حقول المخطط المحوري فقط عندما يكون المخطط PivotChart. |
| [getIs3D()](#getIs3D--) | يشير إلى ما إذا كان المخطط مخططًا ثلاثي الأبعاد. |
| [getLegend()](#getLegend--) | يحصل على مفتاح المخطط. |
| [getLine()](#getLine--) | يحصل على الخط. |
| [getNSeries()](#getNSeries--) | يحصل على مجموعة [SeriesCollection](../../com.aspose.cells/seriescollection) التي تمثل سلسلة البيانات في المخطط. |
| [getName()](#getName--) | يحصل على اسم المخطط. |
| [getPageSetup()](#getPageSetup--) | يمثل وصف إعداد الصفحة في هذا المخطط. |
| [getPerspective()](#getPerspective--) | يرجع أو يضبط المنظور لعرض المخطط three\\u9225\\u6178 dimensional. |
| [getPivotOptions()](#getPivotOptions--) | يحدد عناصر التحكم المحورية التي تظهر على المخطط. |
| [getPivotSource()](#getPivotSource--) | المصدر هو بيانات جدول المحور. |
| [getPlacement()](#getPlacement--) | يمثل الطريقة التي يتم بها إرفاق المخطط بالخلايا تحته. |
| [getPlotArea()](#getPlotArea--) | يحصل على مساحة رسم المخطط التي تشمل تسميات علامات المحور. |
| [getPlotBy()](#getPlotBy--) | يحصل على ما إذا كان المخطط حسب الصف أو العمود. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | يحصل على طريقة رسم الخلايا الفارغة. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | يشير إلى ما إذا كان يتم رسم الخلايا المرئية فقط. |
| [getPlotVisibleCellsOnly()](#getPlotVisibleCellsOnly--) | يشير إلى ما إذا كان يتم رسم الخلايا المرئية فقط. |
| [getPrintSize()](#getPrintSize--) | يحصل على حجم المخطط المطبوع. |
| [getRightAngleAxes()](#getRightAngleAxes--) | صحيح إذا كانت محاور المخطط بزاوية قائمة. |
| [getRotationAngle()](#getRotationAngle--) | يمثل دوران عرض المخطط ثلاثي الأبعاد (دوران منطقة الرسم حول المحور z، بالدرجات). |
| [getSecondCategoryAxis()](#getSecondCategoryAxis--) | يحصل على المحور X الثاني للمخطط. |
| [getSecondValueAxis()](#getSecondValueAxis--) | يحصل على المحور Y الثاني للمخطط. |
| [getSeriesAxis()](#getSeriesAxis--) | يحصل على محور السلسلة للمخطط. |
| [getShapes()](#getShapes--) | يرجع جميع أشكال الرسم في هذا المخطط. |
| [getShowDataTable()](#getShowDataTable--) | يحصل على قيمة تشير إلى ما إذا كان المخطط يعرض جدول بيانات. |
| [getShowLegend()](#getShowLegend--) | يحصل على قيمة تشير إلى ما إذا كان سيتم عرض مفتاح المخطط. |
| [getSideWall()](#getSideWall--) | يرجع كائن [getWalls()](../../com.aspose.cells/chart\#getWalls--) يمثل الجدار الجانبي لمخطط ثلاثي الأبعاد. |
| [getSizeWithWindow()](#getSizeWithWindow--) | صحيح إذا كان Microsoft Excel يعيد تحجيم المخطط ليتطابق مع حجم نافذة ورقة المخطط. |
| [getStyle()](#getStyle--) | يحصل على النمط المدمج. |
| [getSubTitle()](#getSubTitle--) | يحصل على العنوان الفرعي للمخطط. |
| [getTitle()](#getTitle--) | يحصل على عنوان المخطط. |
| [getType()](#getType--) | يحصل على نوع المخطط. |
| [getValueAxis()](#getValueAxis--) | يحصل على المحور Y للمخطط. |
| [getWalls()](#getWalls--) | يرجع كائن [getWalls()](../../com.aspose.cells/chart\#getWalls--) يمثل جدران مخطط ثلاثي الأبعاد. |
| [getWallsAndGridlines2D()](#getWallsAndGridlines2D--) | صحيح إذا تم رسم خطوط الشبكة ثنائي الأبعاد على مخطط ثلاثي الأبعاد. |
| [getWorksheet()](#getWorksheet--) | يحصل على ورقة العمل التي تحتوي على هذا المخطط. |
| [hasAxis(int aixsType, boolean isPrimary)](#hasAxis-int-boolean-) | يرجع المحاور الموجودة على المخطط. |
| [hashCode()](#hashCode--) |  |
| [isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)](#isCellReferedByChart-int-int-int-) | يرجع ما إذا كانت الخلية المشار إليها من قبل المخطط. |
| [isChartDataChanged()](#isChartDataChanged--) | يكشف ما إذا كان مصدر بيانات المخطط قد تغير. |
| [isRectangularCornered()](#isRectangularCornered--) | يحصل على قيمة تشير إلى ما إذا كانت مساحة المخطط ذات زوايا مستطيلة. |
| [isReferedByChart(int rowIndex, int columnIndex)](#isReferedByChart-int-int-) | يعيد ما إذا كانت الخلية مشار إليها من قبل المخطط. |
| [move(int topRow, int leftColumn, int bottomRow, int rightColumn)](#move-int-int-int-int-) | ينقل المخطط إلى موقع محدد. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshPivotData()](#refreshPivotData--) | يقوم بتحديث بيانات المخطط من جدول محوري. |
| [setAutoScaling(boolean value)](#setAutoScaling-boolean-) | صحيح إذا كان Microsoft Excel يضبط مخططًا ثلاثي الأبعاد بحيث يكون حجمه أقرب إلى المخطط الثنائي الأبعاد المكافئ. |
| [setChartDataRange(String area, boolean isVertical)](#setChartDataRange-java.lang.String-boolean-) | يحدد نطاق البيانات للمخطط. |
| [setDepthPercent(int value)](#setDepthPercent-int-) | يمثل عمق المخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 20 و2000 بالمئة). |
| [setDisplayNaAsBlank(boolean value)](#setDisplayNaAsBlank-boolean-) | يشير إلى ما إذا كان يجب عرض \#N/A كقيمة فارغة. |
| [setElevation(int value)](#setElevation-int-) | يمثل ارتفاع عرض المخطط ثلاثي الأبعاد، بالدرجات. |
| [setFirstSliceAngle(int value)](#setFirstSliceAngle-int-) | يضبط زاوية الشريحة الأولى في مخطط الفطيرة أو مخطط الدونات، بالدرجات (عقارب الساعة من العمودي). |
| [setGapDepth(int value)](#setGapDepth-int-) | يضبط المسافة بين سلاسل البيانات في مخطط ثلاثي الأبعاد كنسبة مئوية من عرض العلامة. |
| [setGapWidth(int value)](#setGapWidth-int-) | يرجع أو يضبط المسافة بين مجموعات الأعمدة أو الأشرطة، كنسبة مئوية من عرض العمود أو الشريط. |
| [setHeightPercent(int value)](#setHeightPercent-int-) | يرجع أو يضبط ارتفاع المخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 5 و500 بالمئة). |
| [setHidePivotFieldButtons(boolean value)](#setHidePivotFieldButtons-boolean-) | يشير إلى ما إذا كان يجب إخفاء أزرار حقول المخطط المحوري فقط عندما يكون المخطط PivotChart. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم المخطط. |
| [setPerspective(short value)](#setPerspective-short-) | يرجع أو يضبط المنظور لعرض المخطط three\\u9225\\u6178 dimensional. |
| [setPivotSource(String value)](#setPivotSource-java.lang.String-) | المصدر هو بيانات جدول المحور. |
| [setPlacement(int value)](#setPlacement-int-) | يمثل الطريقة التي يتم بها إرفاق المخطط بالخلايا تحته. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | يضبط طريقة رسم الخلايا الفارغة. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | يشير إلى ما إذا كان يتم رسم الخلايا المرئية فقط. |
| [setPlotVisibleCellsOnly(boolean value)](#setPlotVisibleCellsOnly-boolean-) | يشير إلى ما إذا كان يتم رسم الخلايا المرئية فقط. |
| [setPrintSize(int value)](#setPrintSize-int-) | يضبط حجم المخطط المطبوع. |
| [setRectangularCornered(boolean value)](#setRectangularCornered-boolean-) | يضبط قيمة تشير إلى ما إذا كانت مساحة المخطط ذات زوايا مستطيلة. |
| [setRightAngleAxes(boolean value)](#setRightAngleAxes-boolean-) | صحيح إذا كانت محاور المخطط بزاوية قائمة. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | يمثل دوران عرض المخطط ثلاثي الأبعاد (دوران منطقة الرسم حول المحور z، بالدرجات). |
| [setShowDataTable(boolean value)](#setShowDataTable-boolean-) | يضبط قيمة تشير إلى ما إذا كان المخطط يعرض جدول بيانات. |
| [setShowLegend(boolean value)](#setShowLegend-boolean-) | يضبط قيمة تشير إلى ما إذا كان وسيط المخطط سيظهر. |
| [setSizeWithWindow(boolean value)](#setSizeWithWindow-boolean-) | صحيح إذا كان Microsoft Excel يعيد تحجيم المخطط ليتطابق مع حجم نافذة ورقة المخطط. |
| [setStyle(int value)](#setStyle-int-) | يضبط النمط المدمج. |
| [setType(int value)](#setType-int-) | يضبط نوع المخطط. |
| [setWallsAndGridlines2D(boolean value)](#setWallsAndGridlines2D-boolean-) | صحيح إذا تم رسم خطوط الشبكة ثنائي الأبعاد على مخطط ثلاثي الأبعاد. |
| [switchRowColumn()](#switchRowColumn--) | يبدل الصف/العمود. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | ينشئ صورة المخطط ويحفظها إلى تدفق بالتنسيق المحدد. |
| [toImage(String imageFile)](#toImage-java.lang.String-) | ينشئ صورة المخطط ويحفظها إلى ملف. |
| [toImage(String imageFile, ImageFormat imageFormat)](#toImage-java.lang.String-com.aspose.cells.ImageFormat-) | ينشئ صورة المخطط ويحفظها إلى ملف بالتنسيق المحدد. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | ينشئ صورة المخطط ويحفظها إلى ملف. |
| [toImage(String imageFile, int imageType)](#toImage-java.lang.String-int-) | ينشئ صورة المخطط ويحفظها إلى ملف بنوع الصورة المحدد. |
| [toImage(String imageFile, long jpegQuality)](#toImage-java.lang.String-long-) | ينشئ صورة المخطط ويحفظها إلى ملف بتنسيق Jpeg. |
| [toPdf(OutputStream stream)](#toPdf-java.io.OutputStream-) | ينشئ ملف PDF للمخطط ويحفظه إلى تدفق. |
| [toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.io.OutputStream-float-float-int-int-) | ينشئ ملف PDF للمخطط ويحفظه إلى تدفق. |
| [toPdf(String fileName)](#toPdf-java.lang.String-) | يحفظ المخطط إلى ملف PDF. |
| [toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.lang.String-float-float-int-int-) | يحفظ المخطط إلى ملف PDF. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate() {#calculate--}
```
public void calculate()
```


يحسب المواضع المخصصة لمنطقة الرسم والمحاور إذا تم تعيين مواضعها تلقائيًا.

### calculate(ChartCalculateOptions calculateOptions) {#calculate-com.aspose.cells.ChartCalculateOptions-}
```
public void calculate(ChartCalculateOptions calculateOptions)
```


يحسب الموضع المخصص لمنطقة الرسم والمحاور إذا تم تعيين موضعها تلقائيًا، باستخدام خيارات حساب المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| calculateOptions | [ChartCalculateOptions](../../com.aspose.cells/chartcalculateoptions) |  |

### changeTemplate(byte[] data) {#changeTemplate-byte---}
```
public void changeTemplate(byte[] data)
```


تغيير نوع المخطط باستخدام قالب مسبق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| بيانات | byte[] | بيانات ملف قالب المخطط (.crtx). |

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
### getActualChartSize() {#getActualChartSize--}
```
public int[] getActualChartSize()
```


يحصل على الحجم الفعلي للمخطط بوحدة البكسل.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام طريقة Chart.getActualSize(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int[] - الحجم الفعلي في مصفوفة (العرض والارتفاع). [0] هو العرض؛ [1] هو الارتفاع.
### getActualSize() {#getActualSize--}
```
public int[] getActualSize()
```


يحصل على الحجم الفعلي للمخطط بوحدة البكسل.

**Returns:**
int[] - الحجم الفعلي في مصفوفة (العرض والارتفاع). [0] هو العرض؛ [1] هو الارتفاع.
### getAutoScaling() {#getAutoScaling--}
```
public boolean getAutoScaling()
```


صحيح إذا كان Microsoft Excel يضبط مخططًا ثلاثي الأبعاد بحيث يكون أقرب في الحجم إلى المخطط الثنائي الأبعاد المكافئ. يجب أن تكون خاصية RightAngleAxes صادقة.

**Returns:**
boolean
### getBackWall() {#getBackWall--}
```
public Walls getBackWall()
```


يعيد كائنًا [getWalls()](../../com.aspose.cells/chart\\#getWalls--) يمثل الجدار الخلفي لمخطط ثلاثي الأبعاد.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getCategoryAxis() {#getCategoryAxis--}
```
public Axis getCategoryAxis()
```


يحصل على المحور X للمخطط.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getChartArea() {#getChartArea--}
```
public ChartArea getChartArea()
```


يحصل على مساحة المخطط في ورقة العمل.

**Returns:**
[ChartArea](../../com.aspose.cells/chartarea)
### getChartDataRange() {#getChartDataRange--}
```
public String getChartDataRange()
```


يحصل على نطاق مصدر البيانات للمخطط.

**Remarks**

يدعم النطاق فقط. إذا كانت Series.Values و Name و XValues في نطاق متصل، سيتم إرجاع نطاق يحتويها.

**Returns:**
java.lang.String - مصدر البيانات.
### getChartDataTable() {#getChartDataTable--}
```
public ChartDataTable getChartDataTable()
```


يمثل جدول بيانات المخطط.

**Returns:**
[ChartDataTable](../../com.aspose.cells/chartdatatable)
### getChartObject() {#getChartObject--}
```
public ChartShape getChartObject()
```


يمثل شكل المخطط؛

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getChartShape() {#getChartShape--}
```
public ChartShape getChartShape()
```


يمثل شكل المخطط؛

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية Aspose.Cells.Charts.Chart.ChartObject. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2012. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDepthPercent() {#getDepthPercent--}
```
public int getDepthPercent()
```


يمثل عمق المخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 20 و2000 بالمئة).

**Returns:**
int
### getDisplayNaAsBlank() {#getDisplayNaAsBlank--}
```
public boolean getDisplayNaAsBlank()
```


يشير إلى ما إذا كان يجب عرض \#N/A كقيمة فارغة.

**Returns:**
boolean
### getElevation() {#getElevation--}
```
public int getElevation()
```


يمثل ارتفاع عرض المخطط ثلاثي الأبعاد، بالدرجات.

**Remarks**

ارتفاع المخطط هو الارتفاع الذي تشاهد منه المخطط، بالدرجات. القيمة الافتراضية هي 15 لمعظم أنواع المخططات. يجب أن تكون قيمة هذه الخاصية بين -90 و 90، باستثناء مخططات الأعمدة ثلاثية الأبعاد، حيث يجب أن تكون بين 0 و 44.

**Returns:**
int
### getFilteredNSeries() {#getFilteredNSeries--}
```
public SeriesCollection getFilteredNSeries()
```


يحصل على مجموعة [SeriesCollection](../../com.aspose.cells/seriescollection) التي تمثل سلسلة البيانات التي تم تصفيتها في المخطط.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public int getFirstSliceAngle()
```


يحصل على زاوية الشريحة الأولى من مخطط الفطيرة أو مخطط الدونات، بالدرجات (مع اتجاه عقارب الساعة من العمودي). ينطبق فقط على مخططات الفطيرة، الفطيرة ثلاثية الأبعاد، ومخططات الدونات، من 0 إلى 360.

**Returns:**
int
### getFloor() {#getFloor--}
```
public Floor getFloor()
```


يرجع كائن [getFloor()](../../com.aspose.cells/chart\#getFloor--) الذي يمثل جدران المخطط ثلاثي الأبعاد.

**Remarks**

هذه الخاصية لا تنطبق على مخططات الفطيرة ثلاثية الأبعاد.

**Returns:**
[Floor](../../com.aspose.cells/floor)
### getGapDepth() {#getGapDepth--}
```
public int getGapDepth()
```


يحصل على المسافة بين سلاسل البيانات في مخطط ثلاثي الأبعاد، كنسبة مئوية من عرض العلامة. يجب أن تكون قيمة هذه الخاصية بين 0 و 500.

**Returns:**
int
### getGapWidth() {#getGapWidth--}
```
public int getGapWidth()
```


يعيد أو يضبط المسافة بين مجموعات الأعمدة أو الأعمدة، كنسبة مئوية من عرض العمود أو الشريط. يجب أن تكون قيمة هذه الخاصية بين 0 و 500.

**Returns:**
int
### getHeightPercent() {#getHeightPercent--}
```
public int getHeightPercent()
```


يرجع أو يضبط ارتفاع المخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 5 و500 بالمئة).

**Returns:**
int
### getHidePivotFieldButtons() {#getHidePivotFieldButtons--}
```
public boolean getHidePivotFieldButtons()
```


يشير إلى ما إذا كان يجب إخفاء أزرار حقول المخطط المحوري فقط عندما يكون المخطط PivotChart.

**Returns:**
boolean
### getIs3D() {#getIs3D--}
```
public boolean getIs3D()
```


يشير إلى ما إذا كان المخطط مخططًا ثلاثي الأبعاد.

**Returns:**
boolean
### getLegend() {#getLegend--}
```
public Legend getLegend()
```


يحصل على مفتاح المخطط.

**Returns:**
[Legend](../../com.aspose.cells/legend)
### getLine() {#getLine--}
```
public Line getLine()
```


يحصل على الخط.

**Returns:**
[Line](../../com.aspose.cells/line)
### getNSeries() {#getNSeries--}
```
public SeriesCollection getNSeries()
```


يحصل على مجموعة [SeriesCollection](../../com.aspose.cells/seriescollection) التي تمثل سلسلة البيانات في المخطط.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم المخطط.

**Returns:**
java.lang.String
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


يمثل وصف إعداد الصفحة في هذا المخطط.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPerspective() {#getPerspective--}
```
public short getPerspective()
```


يعيد أو يضبط المنظور لعرض المخطط ثلاث\\u9225\\u6178 الأبعاد. يجب أن يكون بين 0 و 100. يتم تجاهل هذه الخاصية إذا كانت خاصية RightAngleAxes صادقة.

**Returns:**
short
### getPivotOptions() {#getPivotOptions--}
```
public PivotOptions getPivotOptions()
```


يحدد عناصر التحكم المحورية التي تظهر على المخطط.

**Returns:**
[PivotOptions](../../com.aspose.cells/pivotoptions)
### getPivotSource() {#getPivotSource--}
```
public String getPivotSource()
```


المصدر هو بيانات جدول المحور. إذا لم يكن PivotSource فارغًا، فإن المخطط هو PivotChart.

**Remarks**

إذا كان جدول المحور \"PivotTable1\" في ورقة العمل \"Sheet1\" في الملف \"Book1.xls\". يمكن أن يكون pivotSource هو \"[Book1.xls]Sheet1!PivotTable1\" إذا لم يكن المخطط وجدول المحور في نفس المصنف. إذا قمت بتعيين هذه الخاصية، سيتم فقدان إعداد مصدر البيانات السابق.

**Returns:**
java.lang.String
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


يمثل الطريقة التي يتم بها إرفاق المخطط بالخلايا تحته.

انظر [PlacementType](../../com.aspose.cells/placementtype).

**Returns:**
int
### getPlotArea() {#getPlotArea--}
```
public PlotArea getPlotArea()
```


يحصل على مساحة رسم المخطط التي تشمل تسميات علامات المحور.

**Remarks**

**Returns:**
[PlotArea](../../com.aspose.cells/plotarea)
### getPlotBy() {#getPlotBy--}
```
public int getPlotBy()
```


يحصل على ما إذا كان المخطط حسب الصف أو العمود.

انظر [PlotDataByType](../../com.aspose.cells/plotdatabytype).

**Returns:**
int
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


يحصل على طريقة رسم الخلايا الفارغة.

انظر [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


يشير إلى ما إذا كان يتم رسم الخلايا المرئية فقط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية PlotVisibleCellsOnly. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getPlotVisibleCellsOnly() {#getPlotVisibleCellsOnly--}
```
public boolean getPlotVisibleCellsOnly()
```


يشير إلى ما إذا كان يتم رسم الخلايا المرئية فقط.

**Returns:**
boolean
### getPrintSize() {#getPrintSize--}
```
public int getPrintSize()
```


يحصل على حجم المخطط المطبوع.

انظر [PrintSizeType](../../com.aspose.cells/printsizetype).

**Returns:**
int
### getRightAngleAxes() {#getRightAngleAxes--}
```
public boolean getRightAngleAxes()
```


صحيح إذا كانت محاور المخطط بزاوية قائمة. ينطبق فقط على المخططات ثلاثية الأبعاد (باستثناء Column3D ومخططات الفطيرة ثلاثية الأبعاد).

**Remarks**

إذا كانت هذه الخاصية صادقة، يتم تجاهل خاصية Perspective.

**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


يمثل دوران عرض المخطط ثلاثي الأبعاد (دوران منطقة الرسم حول المحور z، بالدرجات).

**Remarks**

يجب أن تكون قيمة هذه الخاصية من 0 إلى 360، باستثناء مخططات الأعمدة ثلاثية الأبعاد، حيث يجب أن تكون القيمة من 0 إلى 44. القيمة الافتراضية هي 20. ينطبق فقط على المخططات ثلاثية الأبعاد.

**Returns:**
int
### getSecondCategoryAxis() {#getSecondCategoryAxis--}
```
public Axis getSecondCategoryAxis()
```


يحصل على المحور X الثاني للمخطط.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSecondValueAxis() {#getSecondValueAxis--}
```
public Axis getSecondValueAxis()
```


يحصل على المحور Y الثاني للمخطط.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSeriesAxis() {#getSeriesAxis--}
```
public Axis getSeriesAxis()
```


يحصل على محور السلسلة للمخطط.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


يرجع جميع أشكال الرسم في هذا المخطط.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTable() {#getShowDataTable--}
```
public boolean getShowDataTable()
```


يحصل على قيمة تشير إلى ما إذا كان المخطط يعرض جدول بيانات.

**Returns:**
boolean
### getShowLegend() {#getShowLegend--}
```
public boolean getShowLegend()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم عرض مفتاح المخطط. القيمة الافتراضية صادقة.

**Returns:**
boolean
### getSideWall() {#getSideWall--}
```
public Walls getSideWall()
```


يرجع كائن [getWalls()](../../com.aspose.cells/chart\#getWalls--) يمثل الجدار الجانبي لمخطط ثلاثي الأبعاد.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getSizeWithWindow() {#getSizeWithWindow--}
```
public boolean getSizeWithWindow()
```


صحيح إذا كان Microsoft Excel يعيد تحجيم المخطط ليتطابق مع حجم نافذة ورقة المخطط.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public int getStyle()
```


يحصل على النمط المدمج.

**Remarks**

يجب أن تكون بين 1 و 48. إرجاع -1 إذا لم يتم تعيينها.

**Returns:**
int
### getSubTitle() {#getSubTitle--}
```
public Title getSubTitle()
```


يحصل على العنوان الفرعي للمخطط. ينطبق فقط على ملفات ODS.

**Returns:**
[Title](../../com.aspose.cells/title)
### getTitle() {#getTitle--}
```
public Title getTitle()
```


يحصل على عنوان المخطط.

**Returns:**
[Title](../../com.aspose.cells/title)
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع المخطط.

انظر إلى [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getValueAxis() {#getValueAxis--}
```
public Axis getValueAxis()
```


يحصل على المحور Y للمخطط.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getWalls() {#getWalls--}
```
public Walls getWalls()
```


يرجع كائن [getWalls()](../../com.aspose.cells/chart\#getWalls--) يمثل جدران مخطط ثلاثي الأبعاد.

**Remarks**

هذه الخاصية لا تنطبق على مخططات الفطيرة ثلاثية الأبعاد.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getWallsAndGridlines2D() {#getWallsAndGridlines2D--}
```
public boolean getWallsAndGridlines2D()
```


صحيح إذا تم رسم خطوط الشبكة ثنائي الأبعاد على مخطط ثلاثي الأبعاد.

**Returns:**
boolean
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


يحصل على ورقة العمل التي تحتوي على هذا المخطط.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasAxis(int aixsType, boolean isPrimary) {#hasAxis-int-boolean-}
```
public boolean hasAxis(int aixsType, boolean isPrimary)
```


يرجع المحاور الموجودة على المخطط.

**Remarks**

عادةً، Pie، PieExploded، PiePie، PieBar، Pie3D، Pie3DExploded، Doughnut، DoughnutExploded لا يحتوي على محور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| aixsType | int |  |
| isPrimary | boolean |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex) {#isCellReferedByChart-int-int-int-}
```
public boolean isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)
```


يرجع ما إذا كانت الخلية المشار إليها من قبل المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | int | المؤشر Sheet.-1 يعني ورقة العمل التي تحتوي على المخطط الحالي. |
| rowIndex | int | مؤشر الصف |
| columnIndex | int | مؤشر العمود |

**Returns:**
boolean -
### isChartDataChanged() {#isChartDataChanged--}
```
public boolean isChartDataChanged()
```


يكشف ما إذا كان مصدر بيانات المخطط قد تغير.

**Remarks**

تكتشف الطريقة التغييرات في مصدر بيانات المخطط قبل تحويل المخطط إلى تنسيق صورة. عند أول استدعاء Chart.toImage، سيتم تسجيل بيانات مصدر المخطط (مثل XValuesParseData، ValuesParseData). قبل استدعاء طريقة Chart.toImage مرة أخرى، استدعِ طريقة IsChartDataChanged للتحقق مما إذا كان المخطط يحتاج إلى إعادة رسم.

**Returns:**
منطقية - تُرجع true إذا تم تغيير المخطط وإلا تُرجع false
### isRectangularCornered() {#isRectangularCornered--}
```
public boolean isRectangularCornered()
```


يحصل على قيمة تشير إلى ما إذا كانت مساحة المخطط ذات زوايا مستطيلة. القيمة الافتراضية هي true.

**Returns:**
boolean
### isReferedByChart(int rowIndex, int columnIndex) {#isReferedByChart-int-int-}
```
public boolean isReferedByChart(int rowIndex, int columnIndex)
```


يعيد ما إذا كانت الخلية مشار إليها من قبل المخطط.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة IsCellReferedByChart(int,int,int). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أبريل 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | مؤشر الصف |
| columnIndex | int | مؤشر العمود |

**Returns:**
boolean -
### move(int topRow, int leftColumn, int bottomRow, int rightColumn) {#move-int-int-int-int-}
```
public void move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```


ينقل المخطط إلى موقع محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| bottomRow | int | فهرس الصف السفلي الأيمن. |
| rightColumn | int | فهرس العمود السفلي الأيمن. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshPivotData() {#refreshPivotData--}
```
public void refreshPivotData()
```


يقوم بتحديث بيانات المخطط من جدول محوري.

**Remarks**

سنجمع البيانات من مصدر البيانات المحوري إلى تقرير الجدول المحوري. تُستخدم هذه الطريقة فقط لجمع جميع البيانات إلى مخطط محوري.

### setAutoScaling(boolean value) {#setAutoScaling-boolean-}
```
public void setAutoScaling(boolean value)
```


صحيح إذا كان Microsoft Excel يضبط مخططًا ثلاثي الأبعاد بحيث يكون أقرب في الحجم إلى المخطط الثنائي الأبعاد المكافئ. يجب أن تكون خاصية RightAngleAxes صادقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setChartDataRange(String area, boolean isVertical) {#setChartDataRange-java.lang.String-boolean-}
```
public void setChartDataRange(String area, boolean isVertical)
```


يحدد نطاق البيانات للمخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| area | java.lang.String | يحدد القيم التي تُرسم منها سلسلة البيانات |
| isVertical | boolean | يحدد ما إذا كان سيتم رسم السلسلة من نطاق قيم الخلايا حسب الصف أو حسب العمود. |

### setDepthPercent(int value) {#setDepthPercent-int-}
```
public void setDepthPercent(int value)
```


يمثل عمق المخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 20 و2000 بالمئة).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDisplayNaAsBlank(boolean value) {#setDisplayNaAsBlank-boolean-}
```
public void setDisplayNaAsBlank(boolean value)
```


يشير إلى ما إذا كان يجب عرض \#N/A كقيمة فارغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setElevation(int value) {#setElevation-int-}
```
public void setElevation(int value)
```


يمثل ارتفاع عرض المخطط ثلاثي الأبعاد، بالدرجات.

**Remarks**

ارتفاع المخطط هو الارتفاع الذي تشاهد منه المخطط، بالدرجات. القيمة الافتراضية هي 15 لمعظم أنواع المخططات. يجب أن تكون قيمة هذه الخاصية بين -90 و 90، باستثناء مخططات الأعمدة ثلاثية الأبعاد، حيث يجب أن تكون بين 0 و 44.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setFirstSliceAngle(int value) {#setFirstSliceAngle-int-}
```
public void setFirstSliceAngle(int value)
```


يضبط زاوية الشريحة الأولى في مخطط الفطيرة أو مخطط الدونات، بالدرجات (مع اتجاه عقارب الساعة من العمودي). ينطبق فقط على مخططات الفطيرة، الفطيرة ثلاثية الأبعاد، ومخططات الدونات، من 0 إلى 360.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setGapDepth(int value) {#setGapDepth-int-}
```
public void setGapDepth(int value)
```


يضبط المسافة بين سلاسل البيانات في مخطط ثلاثي الأبعاد، كنسبة مئوية من عرض العلامة. يجب أن تكون قيمة هذه الخاصية بين 0 و 500.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setGapWidth(int value) {#setGapWidth-int-}
```
public void setGapWidth(int value)
```


يعيد أو يضبط المسافة بين مجموعات الأعمدة أو الأعمدة، كنسبة مئوية من عرض العمود أو الشريط. يجب أن تكون قيمة هذه الخاصية بين 0 و 500.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHeightPercent(int value) {#setHeightPercent-int-}
```
public void setHeightPercent(int value)
```


يرجع أو يضبط ارتفاع المخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 5 و500 بالمئة).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHidePivotFieldButtons(boolean value) {#setHidePivotFieldButtons-boolean-}
```
public void setHidePivotFieldButtons(boolean value)
```


يشير إلى ما إذا كان يجب إخفاء أزرار حقول المخطط المحوري فقط عندما يكون المخطط PivotChart.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يضبط اسم المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPerspective(short value) {#setPerspective-short-}
```
public void setPerspective(short value)
```


يعيد أو يضبط المنظور لعرض المخطط ثلاث\\u9225\\u6178 الأبعاد. يجب أن يكون بين 0 و 100. يتم تجاهل هذه الخاصية إذا كانت خاصية RightAngleAxes صادقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | short |  |

### setPivotSource(String value) {#setPivotSource-java.lang.String-}
```
public void setPivotSource(String value)
```


المصدر هو بيانات جدول المحور. إذا لم يكن PivotSource فارغًا، فإن المخطط هو PivotChart.

**Remarks**

إذا كان جدول المحور \"PivotTable1\" في ورقة العمل \"Sheet1\" في الملف \"Book1.xls\". يمكن أن يكون pivotSource هو \"[Book1.xls]Sheet1!PivotTable1\" إذا لم يكن المخطط وجدول المحور في نفس المصنف. إذا قمت بتعيين هذه الخاصية، سيتم فقدان إعداد مصدر البيانات السابق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


يمثل الطريقة التي يتم بها إرفاق المخطط بالخلايا تحته.

انظر [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


يضبط طريقة رسم الخلايا الفارغة.

انظر [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


يشير إلى ما إذا كان يتم رسم الخلايا المرئية فقط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية PlotVisibleCellsOnly. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPlotVisibleCellsOnly(boolean value) {#setPlotVisibleCellsOnly-boolean-}
```
public void setPlotVisibleCellsOnly(boolean value)
```


يشير إلى ما إذا كان يتم رسم الخلايا المرئية فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPrintSize(int value) {#setPrintSize-int-}
```
public void setPrintSize(int value)
```


يضبط حجم المخطط المطبوع.

انظر [PrintSizeType](../../com.aspose.cells/printsizetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRectangularCornered(boolean value) {#setRectangularCornered-boolean-}
```
public void setRectangularCornered(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت مساحة المخطط ذات زوايا مستطيلة. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRightAngleAxes(boolean value) {#setRightAngleAxes-boolean-}
```
public void setRightAngleAxes(boolean value)
```


صحيح إذا كانت محاور المخطط بزاوية قائمة. ينطبق فقط على المخططات ثلاثية الأبعاد (باستثناء Column3D ومخططات الفطيرة ثلاثية الأبعاد).

**Remarks**

إذا كانت هذه الخاصية صادقة، يتم تجاهل خاصية Perspective.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


يمثل دوران عرض المخطط ثلاثي الأبعاد (دوران منطقة الرسم حول المحور z، بالدرجات).

**Remarks**

يجب أن تكون قيمة هذه الخاصية من 0 إلى 360، باستثناء مخططات الأعمدة ثلاثية الأبعاد، حيث يجب أن تكون القيمة من 0 إلى 44. القيمة الافتراضية هي 20. ينطبق فقط على المخططات ثلاثية الأبعاد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setShowDataTable(boolean value) {#setShowDataTable-boolean-}
```
public void setShowDataTable(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان المخطط يعرض جدول بيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowLegend(boolean value) {#setShowLegend-boolean-}
```
public void setShowLegend(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان وسيلة إيضاح المخطط ستُعرض. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSizeWithWindow(boolean value) {#setSizeWithWindow-boolean-}
```
public void setSizeWithWindow(boolean value)
```


صحيح إذا كان Microsoft Excel يعيد تحجيم المخطط ليتطابق مع حجم نافذة ورقة المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


يضبط النمط المدمج.

**Remarks**

يجب أن تكون بين 1 و 48. إرجاع -1 إذا لم يتم تعيينها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


يضبط نوع المخطط.

انظر إلى [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setWallsAndGridlines2D(boolean value) {#setWallsAndGridlines2D-boolean-}
```
public void setWallsAndGridlines2D(boolean value)
```


صحيح إذا تم رسم خطوط الشبكة ثنائي الأبعاد على مخطط ثلاثي الأبعاد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### switchRowColumn() {#switchRowColumn--}
```
public boolean switchRowColumn()
```


يبدل الصف/العمود.

**Returns:**
منطقية - False يعني فشل تبديل الصف/العمود.
### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


ينشئ صورة المخطط ويحفظها إلى تدفق بالتنسيق المحدد.

**Remarks**

يتم تحديد تنسيق الصورة باستخدام `options.ImageFormat`. الصيغ التالية مدعومة: ImageFormat.Bmp، ImageFormat.Gif، ImageFormat.Png، ImageFormat.Jpeg، ImageFormat.Tiff، ImageFormat.Emf.

إذا كان العرض أو الارتفاع صفرًا أو لم يكن المخطط مدعومًا وفقًا لقائمة المخططات المدعومة، فإن هذه الطريقة لن تفعل شيئًا. يرجى الرجوع إلى [Supported Charts List][] لمزيد من التفاصيل.


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | دفق الإخراج. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | خيارات إضافية لإنشاء الصورة |

### toImage(String imageFile) {#toImage-java.lang.String-}
```
public void toImage(String imageFile)
```


ينشئ صورة المخطط ويحفظها في ملف. امتداد اسم الملف يحدد تنسيق الصورة.

**Remarks**

يتم تحديد تنسيق الصورة باستخدام امتداد اسم الملف. على سبيل المثال، إذا حددت "myfile.png"، فسيتم حفظ الصورة بتنسيق PNG. الامتدادات التالية معترف بها: .bmp، .gif، .png، .jpg، .jpeg، .tiff، .tif، .emf.

إذا كان العرض أو الارتفاع صفرًا أو لم يكن المخطط مدعومًا وفقًا لقائمة المخططات المدعومة، فإن هذه الطريقة لن تفعل شيئًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| imageFile | java.lang.String | اسم ملف الصورة مع المسار الكامل. |

### toImage(String imageFile, ImageFormat imageFormat) {#toImage-java.lang.String-com.aspose.cells.ImageFormat-}
```
public void toImage(String imageFile, ImageFormat imageFormat)
```


ينشئ صورة المخطط ويحفظها إلى ملف بالتنسيق المحدد.

**Remarks**

ملاحظة: هذا العنصر أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام طريقة Chart.ToImage(string, ImageType). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| imageFile | java.lang.String | اسم ملف الصورة مع المسار الكامل. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | الصيغة التي سيتم حفظ الصورة بها. |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


ينشئ صورة المخطط ويحفظها في ملف. امتداد اسم الملف يحدد تنسيق الصورة.

**Remarks**

يتم تحديد تنسيق الصورة باستخدام امتداد اسم الملف. على سبيل المثال، إذا حددت "myfile.png"، فسيتم حفظ الصورة بتنسيق PNG. الامتدادات التالية معترف بها: .bmp، .gif، .png، .jpg، .jpeg، .tiff، .tif، .emf.

إذا كان العرض أو الارتفاع صفرًا أو لم يكن المخطط مدعومًا وفقًا لقائمة المخططات المدعومة، فإن هذه الطريقة لن تفعل شيئًا. يرجى الرجوع إلى [Supported Charts List][] لمزيد من التفاصيل.

**Example**

يحفظ إلى تنسيق Tiff بدقة 300 نقطة في البوصة وضغط CCITT4.

```
         ImageOrPrintOptions options = new ImageOrPrintOptions();
         options.setHorizontalResolution(300);
         options.setVerticalResolution(300);
         options.setTiffCompression(TiffCompression.COMPRESSION_CCITT_4);
 
         Workbook book = new Workbook("test.xls");
         book.getWorksheets().get(0).getCharts().get(0).toImage("chart.Tiff", options);
```


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| imageFile | java.lang.String | اسم ملف الصورة مع المسار الكامل. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | خيارات إضافية لإنشاء الصورة |

### toImage(String imageFile, int imageType) {#toImage-java.lang.String-int-}
```
public void toImage(String imageFile, int imageType)
```


ينشئ صورة المخطط ويحفظها إلى ملف بنوع الصورة المحدد.

**Remarks**

يتم تحديد نوع الصورة باستخدام `imageType`. الأنواع التالية مدعومة: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

إذا كان العرض أو الارتفاع صفرًا أو لم يكن المخطط مدعومًا وفقًا لقائمة المخططات المدعومة، فإن هذه الطريقة لن تفعل شيئًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| imageFile | java.lang.String | اسم ملف الصورة مع المسار الكامل. |
| imageType | int | [ImageType](../../com.aspose.cells/imagetype). نوع الصورة الذي سيتم حفظ الصورة به. |

### toImage(String imageFile, long jpegQuality) {#toImage-java.lang.String-long-}
```
public void toImage(String imageFile, long jpegQuality)
```


ينشئ صورة المخطط ويحفظها إلى ملف بتنسيق Jpeg.

**Remarks**

إذا كان العرض أو الارتفاع صفرًا أو إذا لم يكن المخطط مدعومًا وفقًا لقائمة المخططات المدعومة، فإن هذه الطريقة لن تقوم بأي شيء. ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة ToImage(string,ImageOrPrintOptions) مع الجودة المحددة. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ مارس 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| imageFile | java.lang.String | اسم ملف الصورة مع المسار الكامل. |
| jpegQuality | long | جودة Jpeg. |

### toPdf(OutputStream stream) {#toPdf-java.io.OutputStream-}
```
public void toPdf(OutputStream stream)
```


ينشئ ملف PDF للمخطط ويحفظه إلى تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | دفق الإخراج. |

### toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.io.OutputStream-float-float-int-int-}
```
public void toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


ينشئ ملف PDF للمخطط ويحفظه إلى تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | دفق الإخراج. |
| desiredPageWidth | float | عرض الصفحة المطلوب بالبوصة. |
| desiredPageHeight | float | ارتفاع الصفحة المطلوب بالبوصة. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). نوع محاذاة المخطط الأفقي في صفحة الإخراج. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). نوع محاذاة المخطط العمودي في صفحة الإخراج. |

### toPdf(String fileName) {#toPdf-java.lang.String-}
```
public void toPdf(String fileName)
```


يحفظ المخطط إلى ملف PDF.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم ملف PDF مع المسار الكامل |

### toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.lang.String-float-float-int-int-}
```
public void toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


يحفظ المخطط إلى ملف PDF.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم ملف PDF مع المسار الكامل |
| desiredPageWidth | float | عرض الصفحة المطلوب بالبوصة. |
| desiredPageHeight | float | ارتفاع الصفحة المطلوب بالبوصة. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). نوع محاذاة المخطط الأفقي في صفحة الإخراج. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). نوع محاذاة المخطط العمودي في صفحة الإخراج. |

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

