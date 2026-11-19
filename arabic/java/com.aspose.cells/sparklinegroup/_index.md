---
title: "SparklineGroup"
second_title: "Aspose.Cells for Java API Reference"
description: "منظم في مجموعة sparkline."
type: docs
url: /ar/java/com.aspose.cells/sparklinegroup/
---

**Inheritance:**
java.lang.Object
```
public class SparklineGroup
```

[Sparkline](../../com.aspose.cells/sparkline) is organized into a sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, "A1:D1", false, ca);
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         // Create CellsColor
         CellsColor clr = book.createCellsColor();
         clr.setColor(Color.getOrange());
         group.setSeriesColor(clr);
 
         // set the high points are colored green and the low points are colored red
         group.setShowHighPoint(true);
         group.setShowLowPoint(true);
         group.getHighPointColor().setColor(Color.getGreen());
         group.getLowPointColor().setColor(Color.getRed());
         // set line weight 
         group.setLineWeight(1.0);
         book.save("output.xlsx", SaveFormat.XLSX);
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDisplayHidden()](#getDisplayHidden--) | يشير إلى ما إذا كان يجب عرض البيانات في الصفوف والأعمدة المخفية. |
| [getFirstPointColor()](#getFirstPointColor--) | يحصل على لون النقطة الأولى للبيانات في مجموعة sparkline. |
| [getHighPointColor()](#getHighPointColor--) | يحصل على لون أعلى نقاط البيانات في مجموعة sparkline. |
| [getHorizontalAxisColor()](#getHorizontalAxisColor--) | يحصل على لون المحور الأفقي في مجموعة sparkline. |
| [getHorizontalAxisDateRange()](#getHorizontalAxisDateRange--) | يمثل النطاق الذي يحتوي على قيم التاريخ لبيانات sparkline. |
| [getLastPointColor()](#getLastPointColor--) | يحصل على لون النقطة الأخيرة للبيانات في مجموعة sparkline. |
| [getLineWeight()](#getLineWeight--) | يحصل على وزن الخط في كل sparkline خطي داخل مجموعة sparkline، بوحدة النقاط. |
| [getLowPointColor()](#getLowPointColor--) | يحصل على لون أدنى نقاط البيانات في مجموعة sparkline. |
| [getMarkersColor()](#getMarkersColor--) | يحصل على لون النقاط في كل sparkline خطي داخل مجموعة sparkline. |
| [getNegativePointsColor()](#getNegativePointsColor--) | يحصل على لون القيم السلبية في مجموعة sparkline. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | يشير إلى كيفية رسم الخلايا الفارغة. |
| [getPlotRightToLeft()](#getPlotRightToLeft--) | يشير إلى ما إذا كانت بيانات الرسم من اليمين إلى اليسار. |
| [getPresetStyle()](#getPresetStyle--) | يحصل على نوع النمط المسبق لمجموعة sparkline. |
| [getSeriesColor()](#getSeriesColor--) | يحصل على لون الـsparklines في مجموعة sparkline. |
| [getShowFirstPoint()](#getShowFirstPoint--) | يشير إلى ما إذا كان يجب تمييز النقطة الأولى للبيانات في مجموعة sparkline. |
| [getShowHighPoint()](#getShowHighPoint--) | يشير إلى ما إذا كان يجب تمييز أعلى نقاط البيانات في مجموعة sparkline. |
| [getShowHorizontalAxis()](#getShowHorizontalAxis--) | يشير إلى ما إذا كان يجب إظهار المحور الأفقي لـ sparkline. |
| [getShowLastPoint()](#getShowLastPoint--) | يشير إلى ما إذا كان يجب تمييز النقطة الأخيرة للبيانات في مجموعة sparkline. |
| [getShowLowPoint()](#getShowLowPoint--) | يشير إلى ما إذا كان يجب تمييز أدنى نقاط البيانات في مجموعة sparkline. |
| [getShowMarkers()](#getShowMarkers--) | يشير إلى ما إذا كان يجب تمييز كل نقطة في كل sparkline خطي في مجموعة sparkline. |
| [getShowNegativePoints()](#getShowNegativePoints--) | يشير إلى ما إذا كان يجب تمييز القيم السلبية في مجموعة sparkline بلون أو علامة مختلفة. |
| [getSparklineCollection()](#getSparklineCollection--) | يحصل على مجموعة كائنات [Sparkline](../../com.aspose.cells/sparkline). |
| [getSparklines()](#getSparklines--) | يحصل على مجموعة كائنات [Sparkline](../../com.aspose.cells/sparkline). |
| [getType()](#getType--) | يشير إلى نوع sparkline لمجموعة sparkline. |
| [getVerticalAxisMaxValue()](#getVerticalAxisMaxValue--) | يحصل على القيمة القصوى المخصصة للمحور العمودي. |
| [getVerticalAxisMaxValueType()](#getVerticalAxisMaxValueType--) | يمثل نوع القيمة القصوى للمحور العمودي. |
| [getVerticalAxisMinValue()](#getVerticalAxisMinValue--) | يحصل على القيمة الدنيا المخصصة للمحور العمودي. |
| [getVerticalAxisMinValueType()](#getVerticalAxisMinValueType--) | يمثل نوع القيمة الدنيا للمحور العمودي. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [resetRanges(String dataRange, boolean isVertical, CellArea locationRange)](#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-) | يعيد تعيين نطاق البيانات ونطاق الموقع لمجموعة sparkline. |
| [setDisplayHidden(boolean value)](#setDisplayHidden-boolean-) | يشير إلى ما إذا كان يجب عرض البيانات في الصفوف والأعمدة المخفية. |
| [setFirstPointColor(CellsColor value)](#setFirstPointColor-com.aspose.cells.CellsColor-) | يضبط لون النقطة الأولى للبيانات في مجموعة sparkline. |
| [setHighPointColor(CellsColor value)](#setHighPointColor-com.aspose.cells.CellsColor-) | يضبط لون أعلى نقاط البيانات في مجموعة sparkline. |
| [setHorizontalAxisColor(CellsColor value)](#setHorizontalAxisColor-com.aspose.cells.CellsColor-) | يضبط لون المحور الأفقي في مجموعة sparkline. |
| [setHorizontalAxisDateRange(String value)](#setHorizontalAxisDateRange-java.lang.String-) | يمثل النطاق الذي يحتوي على قيم التاريخ لبيانات sparkline. |
| [setLastPointColor(CellsColor value)](#setLastPointColor-com.aspose.cells.CellsColor-) | يضبط لون النقطة الأخيرة للبيانات في مجموعة sparkline. |
| [setLineWeight(double value)](#setLineWeight-double-) | يضبط وزن الخط في كل sparkline خطي في مجموعة sparkline، بوحدة النقاط. |
| [setLowPointColor(CellsColor value)](#setLowPointColor-com.aspose.cells.CellsColor-) | يضبط لون أدنى نقاط البيانات في مجموعة sparkline. |
| [setMarkersColor(CellsColor value)](#setMarkersColor-com.aspose.cells.CellsColor-) | يضبط لون النقاط في كل sparkline خطي في مجموعة sparkline. |
| [setNegativePointsColor(CellsColor value)](#setNegativePointsColor-com.aspose.cells.CellsColor-) | يضبط لون القيم السلبية في مجموعة sparkline. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | يشير إلى كيفية رسم الخلايا الفارغة. |
| [setPlotRightToLeft(boolean value)](#setPlotRightToLeft-boolean-) | يشير إلى ما إذا كانت بيانات الرسم من اليمين إلى اليسار. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | يضبط نوع النمط المسبق لمجموعة sparkline. |
| [setSeriesColor(CellsColor value)](#setSeriesColor-com.aspose.cells.CellsColor-) | يضبط لون sparklines في مجموعة sparkline. |
| [setShowFirstPoint(boolean value)](#setShowFirstPoint-boolean-) | يشير إلى ما إذا كان يجب تمييز النقطة الأولى للبيانات في مجموعة sparkline. |
| [setShowHighPoint(boolean value)](#setShowHighPoint-boolean-) | يشير إلى ما إذا كان يجب تمييز أعلى نقاط البيانات في مجموعة sparkline. |
| [setShowHorizontalAxis(boolean value)](#setShowHorizontalAxis-boolean-) | يشير إلى ما إذا كان يجب إظهار المحور الأفقي لـ sparkline. |
| [setShowLastPoint(boolean value)](#setShowLastPoint-boolean-) | يشير إلى ما إذا كان يجب تمييز النقطة الأخيرة للبيانات في مجموعة sparkline. |
| [setShowLowPoint(boolean value)](#setShowLowPoint-boolean-) | يشير إلى ما إذا كان يجب تمييز أدنى نقاط البيانات في مجموعة sparkline. |
| [setShowMarkers(boolean value)](#setShowMarkers-boolean-) | يشير إلى ما إذا كان يجب تمييز كل نقطة في كل sparkline خطي في مجموعة sparkline. |
| [setShowNegativePoints(boolean value)](#setShowNegativePoints-boolean-) | يشير إلى ما إذا كان يجب تمييز القيم السلبية في مجموعة sparkline بلون أو علامة مختلفة. |
| [setType(int value)](#setType-int-) | يشير إلى نوع sparkline لمجموعة sparkline. |
| [setVerticalAxisMaxValue(double value)](#setVerticalAxisMaxValue-double-) | يضبط القيمة القصوى المخصصة للمحور العمودي. |
| [setVerticalAxisMaxValue(int type, double value)](#setVerticalAxisMaxValue-int-double-) | يضبط القيمة القصوى المخصصة للمحور العمودي لـ sparkline مع نوع قيمة المحور المحدد. |
| [setVerticalAxisMaxValueType(int value)](#setVerticalAxisMaxValueType-int-) | يمثل نوع القيمة القصوى للمحور العمودي. |
| [setVerticalAxisMinValue(double value)](#setVerticalAxisMinValue-double-) | يضبط القيمة الدنيا المخصصة للمحور العمودي. |
| [setVerticalAxisMinValue(int type, double value)](#setVerticalAxisMinValue-int-double-) | يضبط القيمة الدنيا المخصصة للمحور العمودي للخط الصغير مع نوع قيمة المحور المحدد. |
| [setVerticalAxisMinValueType(int value)](#setVerticalAxisMinValueType-int-) | يمثل نوع القيمة الدنيا للمحور العمودي. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDisplayHidden() {#getDisplayHidden--}
```
public boolean getDisplayHidden()
```


يشير إلى ما إذا كان يجب عرض البيانات في الصفوف والأعمدة المخفية.

**Returns:**
boolean
### getFirstPointColor() {#getFirstPointColor--}
```
public CellsColor getFirstPointColor()
```


يحصل على لون النقطة الأولى للبيانات في مجموعة sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHighPointColor() {#getHighPointColor--}
```
public CellsColor getHighPointColor()
```


يحصل على لون أعلى نقاط البيانات في مجموعة sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisColor() {#getHorizontalAxisColor--}
```
public CellsColor getHorizontalAxisColor()
```


يحصل على لون المحور الأفقي في مجموعة sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisDateRange() {#getHorizontalAxisDateRange--}
```
public String getHorizontalAxisDateRange()
```


يمثل النطاق الذي يحتوي على قيم التاريخ لبيانات sparkline.

**Returns:**
java.lang.String
### getLastPointColor() {#getLastPointColor--}
```
public CellsColor getLastPointColor()
```


يحصل على لون النقطة الأخيرة للبيانات في مجموعة sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getLineWeight() {#getLineWeight--}
```
public double getLineWeight()
```


يحصل على وزن الخط في كل sparkline خطي داخل مجموعة sparkline، بوحدة النقاط.

**Returns:**
double
### getLowPointColor() {#getLowPointColor--}
```
public CellsColor getLowPointColor()
```


يحصل على لون أدنى نقاط البيانات في مجموعة sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getMarkersColor() {#getMarkersColor--}
```
public CellsColor getMarkersColor()
```


يحصل على لون النقاط في كل sparkline خطي داخل مجموعة sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getNegativePointsColor() {#getNegativePointsColor--}
```
public CellsColor getNegativePointsColor()
```


يحصل على لون القيم السلبية في مجموعة sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


يشير إلى كيفية رسم الخلايا الفارغة.

انظر [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotRightToLeft() {#getPlotRightToLeft--}
```
public boolean getPlotRightToLeft()
```


يشير إلى ما إذا كانت بيانات الرسم من اليمين إلى اليسار.

**Returns:**
boolean
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


يحصل على نوع النمط المسبق لمجموعة sparkline.

انظر [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

إذا تم تعيين هذه الخاصية، فإن هذه الخصائص: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor ستُغطى. لذا يرجى تعيين الخاصية أولاً، ثم تعيين البقية.

**Returns:**
int
### getSeriesColor() {#getSeriesColor--}
```
public CellsColor getSeriesColor()
```


يحصل على لون الـsparklines في مجموعة sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getShowFirstPoint() {#getShowFirstPoint--}
```
public boolean getShowFirstPoint()
```


يشير إلى ما إذا كان يجب تمييز النقطة الأولى للبيانات في مجموعة sparkline.

**Returns:**
boolean
### getShowHighPoint() {#getShowHighPoint--}
```
public boolean getShowHighPoint()
```


يشير إلى ما إذا كان يجب تمييز أعلى نقاط البيانات في مجموعة sparkline.

**Returns:**
boolean
### getShowHorizontalAxis() {#getShowHorizontalAxis--}
```
public boolean getShowHorizontalAxis()
```


يشير إلى ما إذا كان يجب إظهار المحور الأفقي للخط الصغير. يظهر المحور الأفقي إذا كان للخط الصغير بيانات تتقاطع مع محور الصفر.

**Returns:**
boolean
### getShowLastPoint() {#getShowLastPoint--}
```
public boolean getShowLastPoint()
```


يشير إلى ما إذا كان يجب تمييز النقطة الأخيرة للبيانات في مجموعة sparkline.

**Returns:**
boolean
### getShowLowPoint() {#getShowLowPoint--}
```
public boolean getShowLowPoint()
```


يشير إلى ما إذا كان يجب تمييز أدنى نقاط البيانات في مجموعة sparkline.

**Returns:**
boolean
### getShowMarkers() {#getShowMarkers--}
```
public boolean getShowMarkers()
```


يشير إلى ما إذا كان يجب تمييز كل نقطة في كل sparkline خطي في مجموعة sparkline.

**Returns:**
boolean
### getShowNegativePoints() {#getShowNegativePoints--}
```
public boolean getShowNegativePoints()
```


يشير إلى ما إذا كان يجب تمييز القيم السلبية في مجموعة sparkline بلون أو علامة مختلفة.

**Returns:**
boolean
### getSparklineCollection() {#getSparklineCollection--}
```
public SparklineCollection getSparklineCollection()
```


يحصل على مجموعة كائنات [Sparkline](../../com.aspose.cells/sparkline).

**Remarks**

ملاحظة: هذه العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام الخاصية SparklineGroup.Sparklines. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ نوفمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getSparklines() {#getSparklines--}
```
public SparklineCollection getSparklines()
```


يحصل على مجموعة كائنات [Sparkline](../../com.aspose.cells/sparkline).

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getType() {#getType--}
```
public int getType()
```


يشير إلى نوع sparkline لمجموعة sparkline.

انظر [SparklineType](../../com.aspose.cells/sparklinetype).

**Returns:**
int
### getVerticalAxisMaxValue() {#getVerticalAxisMaxValue--}
```
public double getVerticalAxisMaxValue()
```


يحصل على القيمة القصوى المخصصة للمحور العمودي.

**Remarks**

إذا تم تعيين هذه الخاصية، فإن [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) سيصبح [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Returns:**
double
### getVerticalAxisMaxValueType() {#getVerticalAxisMaxValueType--}
```
public int getVerticalAxisMaxValueType()
```


يمثل نوع القيمة القصوى للمحور العمودي.

انظر [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Returns:**
int
### getVerticalAxisMinValue() {#getVerticalAxisMinValue--}
```
public double getVerticalAxisMinValue()
```


يحصل على القيمة الدنيا المخصصة للمحور العمودي.

**Remarks**

إذا تم تعيين هذه الخاصية، فإن [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) سيصبح [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Returns:**
double
### getVerticalAxisMinValueType() {#getVerticalAxisMinValueType--}
```
public int getVerticalAxisMinValueType()
```


يمثل نوع القيمة الدنيا للمحور العمودي.

انظر [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### resetRanges(String dataRange, boolean isVertical, CellArea locationRange) {#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-}
```
public void resetRanges(String dataRange, boolean isVertical, CellArea locationRange)
```


يعيد تعيين نطاق البيانات ونطاق الموقع لمجموعة الخط الصغير. ستقوم هذه الطريقة بمسح عناصر الخط الصغير الأصلية في المجموعة وإنشاء عناصر خط صغير جديدة للنطاقات الجديدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dataRange | java.lang.String | يحدد نطاق البيانات الجديد لمجموعة الخط الصغير. |
| isVertical | boolean | يحدد ما إذا كان سيتم رسم الخطوط الصغيرة من نطاق البيانات الجديد حسب الصف أو حسب العمود. |
| locationRange | [CellArea](../../com.aspose.cells/cellarea) | يحدد مكان وضع الخطوط الصغيرة. |

### setDisplayHidden(boolean value) {#setDisplayHidden-boolean-}
```
public void setDisplayHidden(boolean value)
```


يشير إلى ما إذا كان يجب عرض البيانات في الصفوف والأعمدة المخفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFirstPointColor(CellsColor value) {#setFirstPointColor-com.aspose.cells.CellsColor-}
```
public void setFirstPointColor(CellsColor value)
```


يضبط لون النقطة الأولى للبيانات في مجموعة sparkline.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHighPointColor(CellsColor value) {#setHighPointColor-com.aspose.cells.CellsColor-}
```
public void setHighPointColor(CellsColor value)
```


يضبط لون أعلى نقاط البيانات في مجموعة sparkline.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisColor(CellsColor value) {#setHorizontalAxisColor-com.aspose.cells.CellsColor-}
```
public void setHorizontalAxisColor(CellsColor value)
```


يضبط لون المحور الأفقي في مجموعة sparkline.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisDateRange(String value) {#setHorizontalAxisDateRange-java.lang.String-}
```
public void setHorizontalAxisDateRange(String value)
```


يمثل النطاق الذي يحتوي على قيم التاريخ لبيانات sparkline.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setLastPointColor(CellsColor value) {#setLastPointColor-com.aspose.cells.CellsColor-}
```
public void setLastPointColor(CellsColor value)
```


يضبط لون النقطة الأخيرة للبيانات في مجموعة sparkline.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setLineWeight(double value) {#setLineWeight-double-}
```
public void setLineWeight(double value)
```


يضبط وزن الخط في كل sparkline خطي في مجموعة sparkline، بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setLowPointColor(CellsColor value) {#setLowPointColor-com.aspose.cells.CellsColor-}
```
public void setLowPointColor(CellsColor value)
```


يضبط لون أدنى نقاط البيانات في مجموعة sparkline.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setMarkersColor(CellsColor value) {#setMarkersColor-com.aspose.cells.CellsColor-}
```
public void setMarkersColor(CellsColor value)
```


يضبط لون النقاط في كل sparkline خطي في مجموعة sparkline.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setNegativePointsColor(CellsColor value) {#setNegativePointsColor-com.aspose.cells.CellsColor-}
```
public void setNegativePointsColor(CellsColor value)
```


يضبط لون القيم السلبية في مجموعة sparkline.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


يشير إلى كيفية رسم الخلايا الفارغة.

انظر [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPlotRightToLeft(boolean value) {#setPlotRightToLeft-boolean-}
```
public void setPlotRightToLeft(boolean value)
```


يشير إلى ما إذا كانت بيانات الرسم من اليمين إلى اليسار.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


يضبط نوع النمط المسبق لمجموعة sparkline.

انظر [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

إذا تم تعيين هذه الخاصية، فإن هذه الخصائص: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor ستُغطى. لذا يرجى تعيين الخاصية أولاً، ثم تعيين البقية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSeriesColor(CellsColor value) {#setSeriesColor-com.aspose.cells.CellsColor-}
```
public void setSeriesColor(CellsColor value)
```


يضبط لون sparklines في مجموعة sparkline.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setShowFirstPoint(boolean value) {#setShowFirstPoint-boolean-}
```
public void setShowFirstPoint(boolean value)
```


يشير إلى ما إذا كان يجب تمييز النقطة الأولى للبيانات في مجموعة sparkline.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowHighPoint(boolean value) {#setShowHighPoint-boolean-}
```
public void setShowHighPoint(boolean value)
```


يشير إلى ما إذا كان يجب تمييز أعلى نقاط البيانات في مجموعة sparkline.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowHorizontalAxis(boolean value) {#setShowHorizontalAxis-boolean-}
```
public void setShowHorizontalAxis(boolean value)
```


يشير إلى ما إذا كان يجب إظهار المحور الأفقي للخط الصغير. يظهر المحور الأفقي إذا كان للخط الصغير بيانات تتقاطع مع محور الصفر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowLastPoint(boolean value) {#setShowLastPoint-boolean-}
```
public void setShowLastPoint(boolean value)
```


يشير إلى ما إذا كان يجب تمييز النقطة الأخيرة للبيانات في مجموعة sparkline.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowLowPoint(boolean value) {#setShowLowPoint-boolean-}
```
public void setShowLowPoint(boolean value)
```


يشير إلى ما إذا كان يجب تمييز أدنى نقاط البيانات في مجموعة sparkline.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowMarkers(boolean value) {#setShowMarkers-boolean-}
```
public void setShowMarkers(boolean value)
```


يشير إلى ما إذا كان يجب تمييز كل نقطة في كل sparkline خطي في مجموعة sparkline.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowNegativePoints(boolean value) {#setShowNegativePoints-boolean-}
```
public void setShowNegativePoints(boolean value)
```


يشير إلى ما إذا كان يجب تمييز القيم السلبية في مجموعة sparkline بلون أو علامة مختلفة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


يشير إلى نوع sparkline لمجموعة sparkline.

انظر [SparklineType](../../com.aspose.cells/sparklinetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setVerticalAxisMaxValue(double value) {#setVerticalAxisMaxValue-double-}
```
public void setVerticalAxisMaxValue(double value)
```


يضبط القيمة القصوى المخصصة للمحور العمودي.

**Remarks**

إذا تم تعيين هذه الخاصية، فإن [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) سيصبح [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setVerticalAxisMaxValue(int type, double value) {#setVerticalAxisMaxValue-int-double-}
```
public void setVerticalAxisMaxValue(int type, double value)
```


يضبط القيمة القصوى المخصصة للمحور العمودي لـ sparkline مع نوع قيمة المحور المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). النوع الذي يحدد كيفية تطبيق القيمة القصوى للمحور. |
| value | double | القيمة القصوى المخصصة للمحور العمودي. يتم تجاهلها إذا لم يكن النوع [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM). |

### setVerticalAxisMaxValueType(int value) {#setVerticalAxisMaxValueType-int-}
```
public void setVerticalAxisMaxValueType(int value)
```


يمثل نوع القيمة القصوى للمحور العمودي.

انظر [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setVerticalAxisMinValue(double value) {#setVerticalAxisMinValue-double-}
```
public void setVerticalAxisMinValue(double value)
```


يضبط القيمة الدنيا المخصصة للمحور العمودي.

**Remarks**

إذا تم تعيين هذه الخاصية، فإن [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) سيصبح [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setVerticalAxisMinValue(int type, double value) {#setVerticalAxisMinValue-int-double-}
```
public void setVerticalAxisMinValue(int type, double value)
```


يضبط القيمة الدنيا المخصصة للمحور العمودي للخط الصغير مع نوع قيمة المحور المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). النوع الذي يحدد كيفية تطبيق القيمة الدنيا للمحور. |
| value | double | القيمة الدنيا المخصصة للمحور العمودي. يتم تجاهلها إذا لم يكن النوع [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM). |

### setVerticalAxisMinValueType(int value) {#setVerticalAxisMinValueType-int-}
```
public void setVerticalAxisMinValueType(int value)
```


يمثل نوع القيمة الدنيا للمحور العمودي.

انظر [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

