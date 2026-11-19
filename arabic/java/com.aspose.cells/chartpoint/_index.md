---
title: "ChartPoint"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل نقطة واحدة في سلسلة داخل مخطط."
type: docs
url: /ar/java/com.aspose.cells/chartpoint/
---

**Inheritance:**
java.lang.Object
```
public class ChartPoint
```

يمثل نقطة واحدة في سلسلة داخل مخطط.

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
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArcEndPointXPx()](#getArcEndPointXPx--) | يحصل على إحداثي x للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). |
| [getArcEndPointYPx()](#getArcEndPointYPx--) | يحصل على إحداثي y للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). |
| [getArcStartPointXPx()](#getArcStartPointXPx--) | يحصل على إحداثي x للنقطة البداية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). |
| [getArcStartPointYPx()](#getArcStartPointYPx--) | يحصل على إحداثي y للنقطة البداية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). |
| [getArea()](#getArea--) | يحصل على [getArea()](../../com.aspose.cells/chartpoint\\#getArea--). |
| [getBorder()](#getBorder--) | يحصل على [Line](../../com.aspose.cells/line). |
| [getBorderWidthPx()](#getBorderWidthPx--) | يحصل على عرض الحدود بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [getBottomPointCount()](#getBottomPointCount--) | يحصل على عدد النقاط السفلية بعد استدعاء طريقة Chart.Calculate(). |
| [getBottomPointXPx(int index)](#getBottomPointXPx-int-) | يحصل على إحداثي x للنقطة السفلية للشكل بعد استدعاء طريقة Chart.Calculate(). |
| [getBottomPointYPx(int index)](#getBottomPointYPx-int-) | يحصل على إحداثي y للنقطة السفلية للشكل بعد استدعاء طريقة Chart.Calculate(). |
| [getClass()](#getClass--) |  |
| [getDataLabels()](#getDataLabels--) | يرجع كائنًا من نوع [getDataLabels()](../../com.aspose.cells/chartpoint\\#getDataLabels--) يمثل تسمية البيانات المرتبطة بهذه النقطة في المخطط. |
| [getDoughnutInnerRadius()](#getDoughnutInnerRadius--) | يحصل على نصف القطر الداخلي لشريحة الدونات بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [getEndAngle()](#getEndAngle--) | يحصل على الزاوية النهائية لقسم الفطيرة، مقاسة بالدرجات في اتجاه عقارب الساعة من محور x بعد استدعاء طريقة Chart.Calculate(). |
| [getExplosion()](#getExplosion--) | المسافة بين شريحة الفطيرة المفتوحة ومركز مخطط الفطيرة تُعبّر عنها كنسبة مئوية من قطر الفطيرة. |
| [getInnerArcEndPointXPx()](#getInnerArcEndPointXPx--) | يحصل على إحداثي x للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). |
| [getInnerArcEndPointYPx()](#getInnerArcEndPointYPx--) | يحصل على إحداثي y للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). |
| [getInnerArcStartPointXPx()](#getInnerArcStartPointXPx--) | يحصل على إحداثي x للنقطة البداية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). |
| [getInnerArcStartPointYPx()](#getInnerArcStartPointYPx--) | يحصل على إحداثي y للنقطة البداية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). |
| [getInnerRadiusPx()](#getInnerRadiusPx--) | يحصل على نصف القطر الداخلي لشريحة الدونات بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [getMarker()](#getMarker--) | يحصل على [getMarker()](../../com.aspose.cells/chartpoint\\#getMarker--). |
| [getOnCategoryAxisPointCount()](#getOnCategoryAxisPointCount--) | يحصل على عدد النقاط على محور الفئة بعد استدعاء طريقة Chart.Calculate(). |
| [getOnCategoryAxisPointXPx(int index)](#getOnCategoryAxisPointXPx-int-) | يحصل على إحداثي x للنقطة على محور الفئة بعد استدعاء طريقة Chart.Calculate(). |
| [getOnCategoryAxisPointYPx(int index)](#getOnCategoryAxisPointYPx-int-) | يحصل على إحداثي y للنقطة على محور الفئة بعد استدعاء طريقة Chart.Calculate(). |
| [getRadiusPx()](#getRadiusPx--) | يحصل على نصف القطر للفقاعة أو الفطيرة أو الدونات بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [getShadow()](#getShadow--) | صحيح إذا كان لنقطة المخطط ظل. |
| [getShapeHeight()](#getShapeHeight--) | يحصل على الارتفاع بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [getShapeHeightPx()](#getShapeHeightPx--) | يحصل على الارتفاع بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [getShapeProperties()](#getShapeProperties--) | يحصل على كائن [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) الذي يحتوي على خصائص الشكل البصرية لنقطة المخطط. |
| [getShapeWidth()](#getShapeWidth--) | يحصل على العرض بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [getShapeWidthPx()](#getShapeWidthPx--) | يحصل على العرض بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [getShapeX()](#getShapeX--) | يحصل على إحداثي x للزاوية العليا اليسرى بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [getShapeXPx()](#getShapeXPx--) | يحصل على إحداثي x للزاوية العليا اليسرى بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [getShapeY()](#getShapeY--) | يحصل على إحداثي y للزاوية العلوية اليسرى بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [getShapeYPx()](#getShapeYPx--) | يحصل على إحداثي y للزاوية العلوية اليسرى بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [getStartAngle()](#getStartAngle--) | يحصل على الزاوية الابتدائية لقسم الفطيرة، مقاسة بالدرجات في اتجاه عقارب الساعة من المحور x بعد استدعاء طريقة Chart.Calculate(). |
| [getTopPointCount()](#getTopPointCount--) | يحصل على عدد النقاط العلوية بعد استدعاء طريقة Chart.Calculate(). |
| [getTopPointXPx(int index)](#getTopPointXPx-int-) | يحصل على إحداثي x للنقطة العلوية للشكل بعد استدعاء طريقة Chart.Calculate(). |
| [getTopPointYPx(int index)](#getTopPointYPx-int-) | يحصل على إحداثي y للنقطة العلوية للشكل بعد استدعاء طريقة Chart.Calculate(). |
| [getXValue()](#getXValue--) | يحصل على قيمة X لنقطة المخطط. |
| [getXValueType()](#getXValueType--) | يحصل على نوع قيمة X لنقطة المخطط. |
| [getYValue()](#getYValue--) | يحصل على قيمة Y لنقطة المخطط. |
| [getYValueType()](#getYValueType--) | يحصل على نوع قيمة Y لنقطة المخطط. |
| [hashCode()](#hashCode--) |  |
| [isInSecondaryPlot()](#isInSecondaryPlot--) | يحصل على قيمة تشير إلى ما إذا كانت هذه النقطة البياناتية في الفطيرة أو الشريط الثاني في مخطط فطيرة داخل فطيرة أو شريط داخل مخطط فطيرة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExplosion(int value)](#setExplosion-int-) | المسافة بين شريحة الفطيرة المفتوحة ومركز مخطط الفطيرة تُعبّر عنها كنسبة مئوية من قطر الفطيرة. |
| [setInSecondaryPlot(boolean value)](#setInSecondaryPlot-boolean-) | يضبط قيمة تشير إلى ما إذا كانت هذه النقطة البياناتية في الفطيرة أو الشريط الثاني في مخطط فطيرة داخل فطيرة أو شريط داخل مخطط فطيرة. |
| [setShadow(boolean value)](#setShadow-boolean-) | صحيح إذا كان لنقطة المخطط ظل. |
| [setXValue(Object value)](#setXValue-java.lang.Object-) | يضبط قيمة X لنقطة المخطط. |
| [setYValue(Object value)](#setYValue-java.lang.Object-) | يضبط قيمة Y لنقطة المخطط. |
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
### getArcEndPointXPx() {#getArcEndPointXPx--}
```
public float getArcEndPointXPx()
```


يحصل على إحداثي x للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخططات Pie و Doughnut.

**Returns:**
float
### getArcEndPointYPx() {#getArcEndPointYPx--}
```
public float getArcEndPointYPx()
```


يحصل على إحداثي y للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط Pie و Doughnut.

**Returns:**
float
### getArcStartPointXPx() {#getArcStartPointXPx--}
```
public float getArcStartPointXPx()
```


يحصل على إحداثي x للنقطة الابتدائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخططات Pie و Doughnut.

**Returns:**
float
### getArcStartPointYPx() {#getArcStartPointYPx--}
```
public float getArcStartPointYPx()
```


يحصل على إحداثي y للنقطة الابتدائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط Pie و Doughnut.

**Returns:**
float
### getArea() {#getArea--}
```
public Area getArea()
```


يحصل على [getArea()](../../com.aspose.cells/chartpoint\\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getBorder() {#getBorder--}
```
public Line getBorder()
```


يحصل على [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getBorderWidthPx() {#getBorderWidthPx--}
```
public int getBorderWidthPx()
```


يحصل على عرض الحدود بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getBottomPointCount() {#getBottomPointCount--}
```
public int getBottomPointCount()
```


يحصل على عدد النقاط السفلية بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getBottomPointXPx(int index) {#getBottomPointXPx-int-}
```
public float getBottomPointXPx(int index)
```


يحصل على إحداثي x للنقطة السفلية للشكل بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخططات 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
float
### getBottomPointYPx(int index) {#getBottomPointYPx-int-}
```
public float getBottomPointYPx(int index)
```


يحصل على إحداثي y للنقطة السفلية للشكل بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخططات 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

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


يرجع كائنًا من نوع [getDataLabels()](../../com.aspose.cells/chartpoint\\#getDataLabels--) يمثل تسمية البيانات المرتبطة بهذه النقطة في المخطط.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDoughnutInnerRadius() {#getDoughnutInnerRadius--}
```
public int getDoughnutInnerRadius()
```


يحصل على نصف القطر الداخلي لشريحة الدونات بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط Doughnut.

**Returns:**
int
### getEndAngle() {#getEndAngle--}
```
public float getEndAngle()
```


يحصل على الزاوية النهائية لقسم الفطيرة، مقاسة بالدرجات في اتجاه عقارب الساعة من المحور x بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط Pie.

**Returns:**
float
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


المسافة بين شريحة الفطيرة المفتوحة ومركز مخطط الفطيرة تُعبّر عنها كنسبة مئوية من قطر الفطيرة.

**Returns:**
int
### getInnerArcEndPointXPx() {#getInnerArcEndPointXPx--}
```
public float getInnerArcEndPointXPx()
```


يحصل على إحداثي x للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخططات Doughnut.

**Returns:**
float
### getInnerArcEndPointYPx() {#getInnerArcEndPointYPx--}
```
public float getInnerArcEndPointYPx()
```


يحصل على إحداثي y للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط Doughnut.

**Returns:**
float
### getInnerArcStartPointXPx() {#getInnerArcStartPointXPx--}
```
public float getInnerArcStartPointXPx()
```


يحصل على إحداثي x للنقطة الابتدائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط Doughnut.

**Returns:**
float
### getInnerArcStartPointYPx() {#getInnerArcStartPointYPx--}
```
public float getInnerArcStartPointYPx()
```


يحصل على إحداثي y لنقطة البداية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط الدونت.

**Returns:**
float
### getInnerRadiusPx() {#getInnerRadiusPx--}
```
public int getInnerRadiusPx()
```


يحصل على نصف القطر الداخلي لشريحة الدونت بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط الدونت.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية ChartPoint.DoughnutInnerRadius. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


يحصل على [getMarker()](../../com.aspose.cells/chartpoint\\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getOnCategoryAxisPointCount() {#getOnCategoryAxisPointCount--}
```
public int getOnCategoryAxisPointCount()
```


يحصل على عدد النقاط على محور الفئة بعد استدعاء طريقة Chart.Calculate(). ينطبق فقط على مخططات المنطقة.

**Remarks**

مخطط المنطقة ثنائي الأبعاد يُعيد 1، مخطط المنطقة ثلاثي الأبعاد يُعيد 2.

**Returns:**
int
### getOnCategoryAxisPointXPx(int index) {#getOnCategoryAxisPointXPx-int-}
```
public float getOnCategoryAxisPointXPx(int index)
```


يحصل على إحداثي x للنقطة على محور الفئة بعد استدعاء طريقة Chart.Calculate(). ينطبق فقط على مخطط المنطقة.

**Remarks**

مخطط المنطقة ثنائي الأبعاد: الفهرس هو 0. مخطط المنطقة ثلاثي الأبعاد: الفهرس هو 0 أو 1.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
float
### getOnCategoryAxisPointYPx(int index) {#getOnCategoryAxisPointYPx-int-}
```
public float getOnCategoryAxisPointYPx(int index)
```


يحصل على إحداثي y للنقطة على محور الفئة بعد استدعاء طريقة Chart.Calculate(). ينطبق فقط على مخطط المنطقة.

**Remarks**

مخطط المنطقة ثنائي الأبعاد: الفهرس هو 0. مخطط المنطقة ثلاثي الأبعاد: الفهرس هو 0 أو 1.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
float
### getRadiusPx() {#getRadiusPx--}
```
public int getRadiusPx()
```


يحصل على نصف القطر للفقاعة أو الفطيرة أو الدونات بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


صحيح إذا كان لنقطة المخطط ظل.

**Returns:**
boolean
### getShapeHeight() {#getShapeHeight--}
```
public int getShapeHeight()
```


يحصل على الارتفاع بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getShapeHeightPx() {#getShapeHeightPx--}
```
public int getShapeHeightPx()
```


يحصل على الارتفاع بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


يحصل على كائن [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) الذي يحتوي على خصائص الشكل البصرية لنقطة المخطط.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShapeWidth() {#getShapeWidth--}
```
public int getShapeWidth()
```


يحصل على العرض بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getShapeWidthPx() {#getShapeWidthPx--}
```
public int getShapeWidthPx()
```


يحصل على العرض بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getShapeX() {#getShapeX--}
```
public int getShapeX()
```


يحصل على إحداثي x للزاوية العليا اليسرى بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getShapeXPx() {#getShapeXPx--}
```
public int getShapeXPx()
```


يحصل على إحداثي x للزاوية العليا اليسرى بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getShapeY() {#getShapeY--}
```
public int getShapeY()
```


يحصل على إحداثي y للزاوية العلوية اليسرى بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getShapeYPx() {#getShapeYPx--}
```
public int getShapeYPx()
```


يحصل على إحداثي y للزاوية العلوية اليسرى بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getStartAngle() {#getStartAngle--}
```
public float getStartAngle()
```


يحصل على الزاوية الابتدائية لقسم الفطيرة، مقاسة بالدرجات باتجاه عقارب الساعة من محور x بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط الفطيرة.

**Returns:**
float
### getTopPointCount() {#getTopPointCount--}
```
public int getTopPointCount()
```


يحصل على عدد النقاط العلوية بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getTopPointXPx(int index) {#getTopPointXPx-int-}
```
public float getTopPointXPx(int index)
```


يحصل على إحداثي x للنقطة العليا للشكل بعد استدعاء طريقة Chart.Calculate(). ينطبق على المخططات ثلاثية الأبعاد: Column3D، Bar3D، Cone، Cylinder، Pyramid و Area3D.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
float
### getTopPointYPx(int index) {#getTopPointYPx-int-}
```
public float getTopPointYPx(int index)
```


يحصل على إحداثي y للنقطة العليا للشكل بعد استدعاء طريقة Chart.Calculate(). ينطبق على المخططات ثلاثية الأبعاد: Column3D، Bar3D، Cone، Cylinder، Pyramid، و Area3D.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
float
### getXValue() {#getXValue--}
```
public Object getXValue()
```


يحصل على قيمة X لنقطة المخطط.

**Returns:**
java.lang.Object
### getXValueType() {#getXValueType--}
```
public int getXValueType()
```


يحصل على نوع قيمة X لنقطة المخطط.

انظر [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getYValue() {#getYValue--}
```
public Object getYValue()
```


يحصل على قيمة Y لنقطة المخطط.

**Returns:**
java.lang.Object
### getYValueType() {#getYValueType--}
```
public int getYValueType()
```


يحصل على نوع قيمة Y لنقطة المخطط.

انظر [CellValueType](../../com.aspose.cells/cellvaluetype).

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


يحصل على قيمة تشير إلى ما إذا كانت هذه النقطة البياناتية في الفطيرة أو الشريط الثاني في مخطط فطيرة داخل فطيرة أو شريط داخل مخطط فطيرة.

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


المسافة بين شريحة الفطيرة المفتوحة ومركز مخطط الفطيرة تُعبّر عنها كنسبة مئوية من قطر الفطيرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setInSecondaryPlot(boolean value) {#setInSecondaryPlot-boolean-}
```
public void setInSecondaryPlot(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت هذه النقطة البياناتية في الفطيرة أو الشريط الثاني في مخطط فطيرة داخل فطيرة أو شريط داخل مخطط فطيرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


صحيح إذا كان لنقطة المخطط ظل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setXValue(Object value) {#setXValue-java.lang.Object-}
```
public void setXValue(Object value)
```


يضبط قيمة X لنقطة المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

### setYValue(Object value) {#setYValue-java.lang.Object-}
```
public void setYValue(Object value)
```


يضبط قيمة Y لنقطة المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

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

