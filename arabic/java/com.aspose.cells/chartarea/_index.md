---
title: "ChartArea"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على الكائن الذي يمثل منطقة المخطط في ورقة العمل."
type: docs
url: /ar/java/com.aspose.cells/chartarea/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe)
```
public class ChartArea extends ChartFrame
```

يحتوي على الكائن الذي يمثل منطقة المخطط في ورقة العمل.

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
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         //Getting Chart Area
         ChartArea chartArea = chart.getChartArea();
 
         //Setting the foreground color of the chart area
         chartArea.getArea().setForegroundColor(Color.getYellow());
 
         //Setting Chart Area Shadow
         chartArea.setShadow(true);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | يحصل على [getArea()](../../com.aspose.cells/chartframe\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | صحيح إذا كان النص داخل الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. |
| [getBackground()](#getBackground--) | يحصل على وضع العرض للخلفية. |
| [getBackgroundMode()](#getBackgroundMode--) | يحصل على وضع العرض للخلفية. |
| [getBorder()](#getBorder--) | يحصل على [Line](../../com.aspose.cells/line). |
| [getChart()](#getChart--) | يحصل على المخطط الذي ينتمي إليه هذا الكائن. |
| [getClass()](#getClass--) |  |
| [getDefaultHeight()](#getDefaultHeight--) | يمثل ارتفاع الموضع الافتراضي بوحدة 1/4000 من مساحة المخطط. |
| [getDefaultHeightRatioToChart()](#getDefaultHeightRatioToChart--) | يمثل ارتفاع الموضع الافتراضي بوحدة جزء من مساحة المخطط. |
| [getDefaultWidth()](#getDefaultWidth--) | يمثل عرض الموضع الافتراضي بوحدة 1/4000 من مساحة المخطط. |
| [getDefaultWidthRatioToChart()](#getDefaultWidthRatioToChart--) | يمثل عرض الموضع الافتراضي بوحدات كسر مساحة المخطط. |
| [getDefaultX()](#getDefaultX--) | يمثل إحداثي x للموضع الافتراضي بوحدات 1/4000 من مساحة المخطط. |
| [getDefaultXRatioToChart()](#getDefaultXRatioToChart--) | يمثل إحداثي x للموضع الافتراضي بوحدات كسر مساحة المخطط. |
| [getDefaultY()](#getDefaultY--) | يمثل إحداثي y للموضع الافتراضي بوحدات 1/4000 من مساحة المخطط. |
| [getDefaultYRatioToChart()](#getDefaultYRatioToChart--) | يمثل إحداثي y للموضع الافتراضي بوحدات كسر مساحة المخطط. |
| [getFont()](#getFont--) | يُرجع كائن [getFont()](../../com.aspose.cells/chartarea\\#getFont--) من كائن ChartArea المحدد. |
| [getHeight()](#getHeight--) | يُرجع الإزاحة العمودية من صف الزاوية السفلية\\u9225\\u6186ight، بوحدات 1/4000 من مساحة المخطط. |
| [getHeightPixel()](#getHeightPixel--) | يحصل على ارتفاع الإطار بوحدات البكسل. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | يُرجع الإزاحة العمودية من صف الزاوية السفلية اليمنى، بوحدات نسبة مساحة المخطط. |
| [getShadow()](#getShadow--) | صحيح إذا كان للإطار ظل. |
| [getShapeProperties()](#getShapeProperties--) | يحصل على كائن [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--). |
| [getTextFont()](#getTextFont--) | يحصل على كائن [getFont()](../../com.aspose.cells/chartframe\#getFont--) لكائن ChartFrame المحدد. |
| [getTextOptions()](#getTextOptions--) | يحصل على خيارات النص. |
| [getWidth()](#getWidth--) | يُرجع الإزاحة الأفقية من عمود الزاوية السفلية اليمنى، بوحدات 1/4000 من مساحة المخطط. |
| [getWidthPixel()](#getWidthPixel--) | يحصل على عرض الإطار بوحدات البكسل. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | يُرجع الإزاحة الأفقية من عمود الزاوية السفلية اليمنى، بوحدات نسبة مساحة المخطط. |
| [getX()](#getX--) | يُرجع الإزاحة الأفقية من عمود الزاوية العلوية اليسرى، بوحدات 1/4000 من مساحة المخطط. |
| [getXPixel()](#getXPixel--) | يحصل على إحداثي x للزاوية العلوية اليسرى بوحدات البكسل. |
| [getXRatioToChart()](#getXRatioToChart--) | يُرجع الإزاحة الأفقية من عمود الزاوية العلوية اليسرى، كنسبة من مساحة المخطط. |
| [getY()](#getY--) | يُرجع أو يحدد الإزاحة العمودية من صف الزاوية العلوية اليسرى، بوحدات 1/4000 من مساحة المخطط. |
| [getYPixel()](#getYPixel--) | يحصل على إحداثي y للزاوية العلوية اليسرى بوحدات بكسل. |
| [getYRatioToChart()](#getYRatioToChart--) | يُرجع أو يحدد الإزاحة العمودية من صف الزاوية العلوية اليسرى، بوحدات نسبة مساحة المخطط. |
| [hashCode()](#hashCode--) |  |
| [isAutomaticSize()](#isAutomaticSize--) | يشير إلى ما إذا كان إطار المخطط بحجم تلقائي. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | يشير إلى ما إذا تم تعيين الموضع الافتراضي (DefaultX، DefaultY، DefaultWidth و DefaultHeight). |
| [isInnerMode()](#isInnerMode--) | يشير إلى ما إذا كان حجم مساحة الرسم يشمل علامات الفواصل وعناوين المحاور. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | صحيح إذا كان النص داخل الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | يشير إلى ما إذا كان إطار المخطط بحجم تلقائي. |
| [setBackground(int value)](#setBackground-int-) | يضبط وضع عرض الخلفية. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | يضبط وضع عرض الخلفية. |
| [setHeight(int value)](#setHeight-int-) | يحدد الإزاحة العمودية من صف الزاوية السفلية\\u9225\\u6186ight، بوحدات 1/4000 من مساحة المخطط. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | يضبط ارتفاع الإطار بوحدات بكسل. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | يحدد الإزاحة العمودية من صف الزاوية السفلية اليمنى، بوحدات نسبة مساحة المخطط. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | يشير إلى ما إذا كان حجم مساحة الرسم يشمل علامات الفواصل وعناوين المحاور. |
| [setPositionAuto()](#setPositionAuto--) | ضبط موضع الإطار إلى تلقائي |
| [setShadow(boolean value)](#setShadow-boolean-) | صحيح إذا كان للإطار ظل. |
| [setWidth(int value)](#setWidth-int-) | يحدد الإزاحة الأفقية من عمود الزاوية السفلية اليمنى، بوحدات 1/4000 من مساحة المخطط. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | يضبط عرض الإطار بوحدات البكسل. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | يحدد الإزاحة الأفقية من عمود الزاوية السفلية اليمنى، بوحدات نسبة مساحة المخطط. |
| [setX(int value)](#setX-int-) | يضبط الإزاحة الأفقية من عمود الزاوية العلوية اليسرى، بوحدات 1/4000 من مساحة المخطط. |
| [setXPixel(int value)](#setXPixel-int-) | يضبط إحداثي x للزاوية العلوية اليسرى بوحدات البكسل. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | يضبط الإزاحة الأفقية من عمود الزاوية العلوية اليسرى، كنسبة من مساحة المخطط. |
| [setY(int value)](#setY-int-) | يُرجع أو يحدد الإزاحة العمودية من صف الزاوية العلوية اليسرى، بوحدات 1/4000 من مساحة المخطط. |
| [setYPixel(int value)](#setYPixel-int-) | يضبط إحداثي y للزاوية العلوية اليسرى بوحدات البكسل. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | يُرجع أو يحدد الإزاحة العمودية من صف الزاوية العلوية اليسرى، بوحدات نسبة مساحة المخطط. |
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


يحصل على [getArea()](../../com.aspose.cells/chartframe\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


صحيح إذا كان النص داخل الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. القيمة الافتراضية هي صحيح.

**Returns:**
boolean
### getBackground() {#getBackground--}
```
public int getBackground()
```


يحصل على وضع عرض الخلفية. هذه الخاصية صالحة فقط في Excel 2003 أو الإصدارات الأقدم.

انظر [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام الخاصية ChartFrame.Area.FillFormat.FillType. على سبيل المثال، إذا كنت بحاجة لتعيين BackgroundMode إلى Opaque، يمكنك استخدام الشيفرة التالية: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ JANUARY 2012. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

**Returns:**
int
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


يحصل على وضع عرض الخلفية. هذه الخاصية صالحة فقط في Excel 2003 أو الإصدارات الأقدم.

انظر [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام الخاصية ChartFrame.Area.FillFormat.FillType. على سبيل المثال، إذا كنت بحاجة لتعيين BackgroundMode إلى Opaque، يمكنك استخدام الشيفرة التالية: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ February 2026. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


يحصل على [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getChart() {#getChart--}
```
public Chart getChart()
```


يحصل على المخطط الذي ينتمي إليه هذا الكائن.

**Returns:**
[Chart](../../com.aspose.cells/chart)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultHeight() {#getDefaultHeight--}
```
public int getDefaultHeight()
```


يمثل ارتفاع الموضع الافتراضي بوحدة 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. يرجى استخدام الخاصية ChartFrame.DefaultHeightRatioToChart بدلاً من ذلك. DefaultHeight = (int)(DefaultHeightRatioToChart \* 4000); سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ February 2025. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

**Returns:**
int
### getDefaultHeightRatioToChart() {#getDefaultHeightRatioToChart--}
```
public double getDefaultHeightRatioToChart()
```


يمثل ارتفاع الموضع الافتراضي بوحدة جزء من مساحة المخطط.

**Returns:**
double
### getDefaultWidth() {#getDefaultWidth--}
```
public int getDefaultWidth()
```


يمثل عرض الموضع الافتراضي بوحدة 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. يرجى استخدام الخاصية ChartFrame.DefaultWidthRatioToChart بدلاً من ذلك. DefaultWidth = (int)(DefaultWidthRatioToChart \* 4000); سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ February 2025. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

**Returns:**
int
### getDefaultWidthRatioToChart() {#getDefaultWidthRatioToChart--}
```
public double getDefaultWidthRatioToChart()
```


يمثل عرض الموضع الافتراضي بوحدات كسر مساحة المخطط.

**Returns:**
double
### getDefaultX() {#getDefaultX--}
```
public int getDefaultX()
```


يمثل إحداثي x للموضع الافتراضي بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. يرجى استخدام الخاصية ChartFrame.DefaultXRatioToChart بدلاً من ذلك. DefaultX = (int)(DefaultXRatioToChart \* 4000); سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ February 2025. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

**Returns:**
int
### getDefaultXRatioToChart() {#getDefaultXRatioToChart--}
```
public double getDefaultXRatioToChart()
```


يمثل إحداثي x للموضع الافتراضي بوحدات كسر مساحة المخطط.

**Returns:**
double
### getDefaultY() {#getDefaultY--}
```
public int getDefaultY()
```


يمثل إحداثي y للموضع الافتراضي بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. يرجى استخدام الخاصية ChartFrame.DefaultYRatioToChart بدلاً من ذلك. DefaultY = (int)(DefaultYRatioToChart \* 4000); سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ February 2025. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

**Returns:**
int
### getDefaultYRatioToChart() {#getDefaultYRatioToChart--}
```
public double getDefaultYRatioToChart()
```


يمثل إحداثي y للموضع الافتراضي بوحدات كسر مساحة المخطط.

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


يُرجع كائن [getFont()](../../com.aspose.cells/chartarea\\#getFont--) من كائن ChartArea المحدد.

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


يُرجع الإزاحة العمودية من صف الزاوية السفلية\\u9225\\u6186ight، بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. يرجى استخدام الخاصية ChartArea.HeightRatioToChart بدلاً من ذلك. Height = HeightRatioToChart \* 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


يحصل على ارتفاع الإطار بوحدات البكسل.

**Returns:**
int
### getHeightRatioToChart() {#getHeightRatioToChart--}
```
public double getHeightRatioToChart()
```


يُرجع الإزاحة العمودية من صف الزاوية السفلية اليمنى، بوحدات نسبة مساحة المخطط.

**Returns:**
double
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


صحيح إذا كان للإطار ظل.

**Remarks**

فقط للمخططات في ملف xls.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


يحصل على كائن [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--).

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


يحصل على كائن [getFont()](../../com.aspose.cells/chartframe\#getFont--) لكائن ChartFrame المحدد.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية ChartFrame.Font. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2012. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


يحصل على خيارات النص.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getWidth() {#getWidth--}
```
public int getWidth()
```


يُرجع الإزاحة الأفقية من عمود الزاوية السفلية اليمنى، بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. يرجى استخدام الخاصية ChartArea.WidthRatioToChart بدلاً من ذلك. Width = WidthRatioToChart \* 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


يحصل على عرض الإطار بوحدات البكسل.

**Returns:**
int
### getWidthRatioToChart() {#getWidthRatioToChart--}
```
public double getWidthRatioToChart()
```


يُرجع الإزاحة الأفقية من عمود الزاوية السفلية اليمنى، بوحدات نسبة مساحة المخطط.

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


يُرجع الإزاحة الأفقية من عمود الزاوية العلوية اليسرى، بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. يرجى استخدام الخاصية ChartArea.XRatioToChart بدلاً من ذلك. X = XRatioToChart \* 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


يحصل على إحداثي x للزاوية العلوية اليسرى بوحدات البكسل.

**Returns:**
int
### getXRatioToChart() {#getXRatioToChart--}
```
public double getXRatioToChart()
```


يُرجع الإزاحة الأفقية من عمود الزاوية العلوية اليسرى، كنسبة من مساحة المخطط.

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


يُرجع أو يحدد الإزاحة العمودية من صف الزاوية العلوية اليسرى، بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. يرجى استخدام الخاصية ChartArea.YRatioToChart بدلاً من ذلك. Y = YRatioToChart \* 4000; سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


يحصل على إحداثي y للزاوية العلوية اليسرى بوحدات بكسل.

**Returns:**
int
### getYRatioToChart() {#getYRatioToChart--}
```
public double getYRatioToChart()
```


يُرجع أو يحدد الإزاحة العمودية من صف الزاوية العلوية اليسرى، بوحدات نسبة مساحة المخطط.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutomaticSize() {#isAutomaticSize--}
```
public boolean isAutomaticSize()
```


يشير إلى ما إذا كان إطار المخطط بحجم تلقائي.

**Returns:**
boolean
### isDefaultPosBeSet() {#isDefaultPosBeSet--}
```
public boolean isDefaultPosBeSet()
```


يشير إلى ما إذا تم تعيين الموضع الافتراضي (DefaultX، DefaultY، DefaultWidth و DefaultHeight).

**Returns:**
boolean
### isInnerMode() {#isInnerMode--}
```
public boolean isInnerMode()
```


يشير إلى ما إذا كان حجم مساحة الرسم يشمل علامات الفواصل وعناوين المحاور. القيمة False تعني أن الحجم سيحدد حجم مساحة الرسم، وعلامات الفواصل، وعناوين المحاور.

**Remarks**

فقط لملف Xlsx.

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




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


صحيح إذا كان النص داخل الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. القيمة الافتراضية هي صحيح.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutomaticSize(boolean value) {#setAutomaticSize-boolean-}
```
public void setAutomaticSize(boolean value)
```


يشير إلى ما إذا كان إطار المخطط بحجم تلقائي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBackground(int value) {#setBackground-int-}
```
public void setBackground(int value)
```


يضبط وضع عرض الخلفية. هذه الخاصية صالحة فقط في Excel 2003 أو الإصدارات الأقدم.

انظر [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام الخاصية ChartFrame.Area.FillFormat.FillType. على سبيل المثال، إذا كنت بحاجة لتعيين BackgroundMode إلى Opaque، يمكنك استخدام الشيفرة التالية: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ JANUARY 2012. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


يضبط وضع عرض الخلفية. هذه الخاصية صالحة فقط في Excel 2003 أو الإصدارات الأقدم.

انظر [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام الخاصية ChartFrame.Area.FillFormat.FillType. على سبيل المثال، إذا كنت بحاجة لتعيين BackgroundMode إلى Opaque، يمكنك استخدام الشيفرة التالية: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ February 2026. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


يحدد الإزاحة العمودية من صف الزاوية السفلية\\u9225\\u6186ight، بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. يرجى استخدام الخاصية ChartArea.HeightRatioToChart بدلاً من ذلك. Height = HeightRatioToChart \* 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


يضبط ارتفاع الإطار بوحدات بكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHeightRatioToChart(double value) {#setHeightRatioToChart-double-}
```
public void setHeightRatioToChart(double value)
```


يحدد الإزاحة العمودية من صف الزاوية السفلية اليمنى، بوحدات نسبة مساحة المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setInnerMode(boolean value) {#setInnerMode-boolean-}
```
public void setInnerMode(boolean value)
```


يشير إلى ما إذا كان حجم مساحة الرسم يشمل علامات الفواصل وعناوين المحاور. القيمة False تعني أن الحجم سيحدد حجم مساحة الرسم، وعلامات الفواصل، وعناوين المحاور.

**Remarks**

فقط لملف Xlsx.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


ضبط موضع الإطار إلى تلقائي

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


صحيح إذا كان للإطار ظل.

**Remarks**

فقط للمخططات في ملف xls.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


يحدد الإزاحة الأفقية من عمود الزاوية السفلية اليمنى، بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. يرجى استخدام الخاصية ChartArea.WidthRatioToChart بدلاً من ذلك. Width = WidthRatioToChart \* 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


يضبط عرض الإطار بوحدات البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setWidthRatioToChart(double value) {#setWidthRatioToChart-double-}
```
public void setWidthRatioToChart(double value)
```


يحدد الإزاحة الأفقية من عمود الزاوية السفلية اليمنى، بوحدات نسبة مساحة المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


يضبط الإزاحة الأفقية من عمود الزاوية العلوية اليسرى، بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. يرجى استخدام الخاصية ChartArea.XRatioToChart بدلاً من ذلك. X = XRatioToChart \* 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


يضبط إحداثي x للزاوية العلوية اليسرى بوحدات البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setXRatioToChart(double value) {#setXRatioToChart-double-}
```
public void setXRatioToChart(double value)
```


يضبط الإزاحة الأفقية من عمود الزاوية العلوية اليسرى، كنسبة من مساحة المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


يُرجع أو يحدد الإزاحة العمودية من صف الزاوية العلوية اليسرى، بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. يرجى استخدام الخاصية ChartArea.YRatioToChart بدلاً من ذلك. Y = YRatioToChart \* 4000; سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


يضبط إحداثي y للزاوية العلوية اليسرى بوحدات البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setYRatioToChart(double value) {#setYRatioToChart-double-}
```
public void setYRatioToChart(double value)
```


يُرجع أو يحدد الإزاحة العمودية من صف الزاوية العلوية اليسرى، بوحدات نسبة مساحة المخطط.

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

