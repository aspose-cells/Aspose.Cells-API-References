---
title: "DataLabels"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من جميع كائنات DataLabel للسلسلة المحددة."
type: docs
url: /ar/java/com.aspose.cells/datalabels/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class DataLabels extends ChartTextFrame
```

يحتوي على مجموعة من جميع كائنات DataLabel للسلسلة المحددة.

**Example**

```
         //Set the DataLabels in the chart
         Workbook wb = new Workbook("chart.xlsx");
         Chart chart = wb.getWorksheets().get(0).getCharts().get(0);
         DataLabels datalabels;
         for (int i = 0; i  <chart.getNSeries().getCount(); i++)
         {
             datalabels = chart.getNSeries().get(i).getDataLabels();
             //Set the position of DataLabels
             datalabels.setPosition(LabelPositionType.INSIDE_BASE);
             //Show the category name in the DataLabels
             datalabels.setShowCategoryName(true);
             //Show the value in the DataLabels
             datalabels.setShowValue(true);
             //Not show the percentage in the DataLabels
             datalabels.setShowPercentage(false);
             //Not show the legend key.
             datalabels.setShowLegendKey(false);
         }
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [applyFont()](#applyFont--) | تطبيق الخط الخاص بتسميات البيانات على جميع العقد الفرعية. |
| [characters(int startIndex, int length)](#characters-int-int-) | يرجع كائن Characters يمثل نطاقًا من الأحرف داخل النص. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | يحصل على [getArea()](../../com.aspose.cells/datalabels\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | صحيح إذا كان النص داخل الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. |
| [getBackground()](#getBackground--) | يحصل على وضع العرض للخلفية. |
| [getBackgroundMode()](#getBackgroundMode--) | يحصل على وضع العرض للخلفية |
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
| [getDirectionType()](#getDirectionType--) | يحصل على اتجاه النص. |
| [getFont()](#getFont--) | يحصل على الخط الخاص بـ DataLabels؛ |
| [getHeight()](#getHeight--) | يحصل على ارتفاع الإطار بوحدات 1/4000 من مساحة المخطط. |
| [getHeightPixel()](#getHeightPixel--) | يحصل على ارتفاع الإطار بوحدات البكسل. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | يحصل على ارتفاع الإطار بوحدات نسبة مساحة المخطط. |
| [getLinkedSource()](#getLinkedSource--) | يحصل على مرجع إلى ورقة العمل. |
| [getNumber()](#getNumber--) | يحصل على تنسيق الرقم المدمج. |
| [getNumberFormat()](#getNumberFormat--) | يمثل سلسلة التنسيق لكائن DataLabels. |
| [getNumberFormatLinked()](#getNumberFormatLinked--) | صحيح إذا كان تنسيق الرقم مرتبطًا بالخلايا (بحيث يتغير تنسيق الرقم في التسميات عندما يتغير في الخلايا). |
| [getPosition()](#getPosition--) | يمثل موضع تسمية البيانات. |
| [getReadingOrder()](#getReadingOrder--) | يمثل ترتيب قراءة النص. |
| [getRotationAngle()](#getRotationAngle--) | يمثل زاوية دوران النص. |
| [getSeparatorType()](#getSeparatorType--) | يحصل على نوع الفاصل المستخدم لتسميات البيانات في المخطط. |
| [getSeparatorValue()](#getSeparatorValue--) | يحصل على قيمة الفاصل المستخدمة لتسميات البيانات في المخطط. |
| [getShadow()](#getShadow--) | صحيح إذا كان للإطار ظل. |
| [getShapeProperties()](#getShapeProperties--) | يحصل على كائن [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--). |
| [getShapeType()](#getShapeType--) | يحصل على نوع الشكل لتسمية البيانات. |
| [getShowBubbleSize()](#getShowBubbleSize--) | يمثل سلوك عرض قيمة النسبة المئوية لتسمية البيانات في مخطط محدد. |
| [getShowCategoryName()](#getShowCategoryName--) | يمثل سلوك عرض اسم الفئة لتسمية البيانات في مخطط محدد. صحيح لعرض اسم الفئة لتسميات البيانات في المخطط. |
| [getShowCellRange()](#getShowCellRange--) | يشير إلى ما إذا كان سيتم عرض نطاق الخلايا كتسميات للبيانات. |
| [getShowLegendKey()](#getShowLegendKey--) | يمثل سلوك عرض مفتاح وسيلة الإيضاح لتسمية البيانات في مخطط محدد. |
| [getShowPercentage()](#getShowPercentage--) | يمثل سلوك عرض قيمة النسبة المئوية لتسمية البيانات في مخطط محدد. |
| [getShowSeriesName()](#getShowSeriesName--) | يشير إلى ما إذا كان اسم السلسلة يُعرض على تسميات البيانات في المخطط. |
| [getShowValue()](#getShowValue--) | يمثل سلوك عرض قيم تسمية البيانات في مخطط محدد. |
| [getText()](#getText--) | يحصل على نص تسمية البيانات. |
| [getTextDirection()](#getTextDirection--) | يمثل ترتيب قراءة النص. |
| [getTextFont()](#getTextFont--) | يحصل على كائن [getFont()](../../com.aspose.cells/chartframe\#getFont--) لكائن ChartFrame المحدد. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | يحصل على محاذاة النص أفقياً. |
| [getTextOptions()](#getTextOptions--) | يحصل على خيارات النص. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | يحصل على محاذاة النص عمودياً. |
| [getWidth()](#getWidth--) | يحصل على عرض الإطار بوحدات 1/4000 من مساحة المخطط. |
| [getWidthPixel()](#getWidthPixel--) | يحصل على عرض الإطار بوحدات البكسل. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | يحصل على عرض الإطار بوحدات نسبة مساحة المخطط. |
| [getX()](#getX--) | يحصل على إحداثي x للزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| [getXPixel()](#getXPixel--) | يحصل على إحداثي x للزاوية العلوية اليسرى بوحدات البكسل. |
| [getXRatioToChart()](#getXRatioToChart--) | يحصل على إحداثي x للزاوية العلوية اليسرى بوحدات نسبة مساحة المخطط. |
| [getY()](#getY--) | يحصل على إحداثي y للزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| [getYPixel()](#getYPixel--) | يحصل على إحداثي y للزاوية العلوية اليسرى بوحدات بكسل. |
| [getYRatioToChart()](#getYRatioToChart--) | يحصل على إحداثي y للزاوية العلوية اليسرى بوحدات نسبة مساحة المخطط. |
| [hashCode()](#hashCode--) |  |
| [isAutoText()](#isAutoText--) | يشير إلى أن النص تم إنشاؤه تلقائيًا. |
| [isAutomaticRotation()](#isAutomaticRotation--) | يشير إلى ما إذا كان نص المخطط يدور تلقائيًا. |
| [isAutomaticSize()](#isAutomaticSize--) | يشير إلى ما إذا كان إطار المخطط بحجم تلقائي. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | يشير إلى ما إذا تم تعيين الموضع الافتراضي (DefaultX، DefaultY، DefaultWidth و DefaultHeight). |
| [isDeleted()](#isDeleted--) | يشير إلى ما إذا تم حذف تسمية البيانات هذه. |
| [isInnerMode()](#isInnerMode--) | يشير إلى ما إذا كان حجم مساحة الرسم يشمل علامات الفواصل وعناوين المحاور. |
| [isNeverOverlap()](#isNeverOverlap--) | يشير إلى ما إذا كانت تسميات البيانات لا تتداخل أبدًا عند تحويل مخطط دائري إلى صورة. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | يحصل على ما إذا كان يجب أن يتناسب الشكل تلقائيًا لاحتواء النص الموصوف داخله بالكامل. |
| [isTextWrapped()](#isTextWrapped--) | يحصل على قيمة تشير إلى ما إذا كان النص مُلتفًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | صحيح إذا كان النص داخل الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. |
| [setAutoText(boolean value)](#setAutoText-boolean-) | يشير إلى أن النص تم إنشاؤه تلقائيًا. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | يشير إلى ما إذا كان إطار المخطط بحجم تلقائي. |
| [setBackground(int value)](#setBackground-int-) | يضبط وضع عرض الخلفية. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | يضبط وضع العرض للخلفية |
| [setDeleted(boolean value)](#setDeleted-boolean-) | يشير إلى ما إذا تم حذف تسمية البيانات هذه. |
| [setDirectionType(int value)](#setDirectionType-int-) | يضبط اتجاه النص. |
| [setHeight(int value)](#setHeight-int-) | يضبط ارتفاع الإطار بوحدات 1/4000 من مساحة المخطط. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | يضبط ارتفاع الإطار بوحدات بكسل. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | يضبط ارتفاع الإطار بوحدات نسبة مساحة المخطط. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | يشير إلى ما إذا كان حجم مساحة الرسم يشمل علامات الفواصل وعناوين المحاور. |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | يضبط مرجعًا إلى ورقة العمل. |
| [setNeverOverlap(boolean value)](#setNeverOverlap-boolean-) | يشير إلى ما إذا كانت تسميات البيانات لا تتداخل أبدًا عند تحويل مخطط دائري إلى صورة. |
| [setNumber(int value)](#setNumber-int-) | يضبط تنسيق الرقم المدمج. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | يمثل سلسلة التنسيق لكائن DataLabels. |
| [setNumberFormatLinked(boolean value)](#setNumberFormatLinked-boolean-) | صحيح إذا كان تنسيق الرقم مرتبطًا بالخلايا (بحيث يتغير تنسيق الرقم في التسميات عندما يتغير في الخلايا). |
| [setPosition(int value)](#setPosition-int-) | يمثل موضع تسمية البيانات. |
| [setPositionAuto()](#setPositionAuto--) | ضبط موضع الإطار إلى تلقائي |
| [setReadingOrder(int value)](#setReadingOrder-int-) | يمثل ترتيب قراءة النص. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | يضبط ما إذا كان يجب أن يتناسب الشكل تلقائيًا لاحتواء النص الموصوف داخله بالكامل. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | يمثل زاوية دوران النص. |
| [setSeparatorType(int value)](#setSeparatorType-int-) | يضبط نوع الفاصل المستخدم لتسميات البيانات في المخطط. |
| [setSeparatorValue(String value)](#setSeparatorValue-java.lang.String-) | يضبط قيمة الفاصل المستخدمة لتسميات البيانات في المخطط. |
| [setShadow(boolean value)](#setShadow-boolean-) | صحيح إذا كان للإطار ظل. |
| [setShapeType(int value)](#setShapeType-int-) | يضبط نوع الشكل لتسمية البيانات. |
| [setShowBubbleSize(boolean value)](#setShowBubbleSize-boolean-) | يمثل سلوك عرض قيمة النسبة المئوية لتسمية البيانات في مخطط محدد. |
| [setShowCategoryName(boolean value)](#setShowCategoryName-boolean-) | يمثل سلوك عرض اسم الفئة لتسمية البيانات في مخطط محدد. صحيح لعرض اسم الفئة لتسميات البيانات في المخطط. |
| [setShowCellRange(boolean value)](#setShowCellRange-boolean-) | يشير إلى ما إذا كان سيتم عرض نطاق الخلايا كتسميات للبيانات. |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | يمثل سلوك عرض مفتاح وسيلة الإيضاح لتسمية البيانات في مخطط محدد. |
| [setShowPercentage(boolean value)](#setShowPercentage-boolean-) | يمثل سلوك عرض قيمة النسبة المئوية لتسمية البيانات في مخطط محدد. |
| [setShowSeriesName(boolean value)](#setShowSeriesName-boolean-) | يشير إلى ما إذا كان اسم السلسلة يُعرض على تسميات البيانات في المخطط. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | يمثل سلوك عرض قيم تسمية البيانات في مخطط محدد. |
| [setText(String value)](#setText-java.lang.String-) | يضبط نص تسمية البيانات. |
| [setTextDirection(int value)](#setTextDirection-int-) | يمثل ترتيب قراءة النص. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | يضبط محاذاة النص أفقياً. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | يضبط محاذاة النص عموديًا. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | يضبط قيمة تشير إلى ما إذا كان النص مُلتفًا. |
| [setWidth(int value)](#setWidth-int-) | يضبط عرض الإطار بوحدات 1/4000 من مساحة المخطط. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | يضبط عرض الإطار بوحدات البكسل. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | يضبط عرض الإطار بوحدات نسبة مساحة المخطط. |
| [setX(int value)](#setX-int-) | يضبط إحداثي x للزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| [setXPixel(int value)](#setXPixel-int-) | يضبط إحداثي x للزاوية العلوية اليسرى بوحدات البكسل. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | يضبط إحداثي x للزاوية العلوية اليسرى بوحدات نسبة مساحة المخطط. |
| [setY(int value)](#setY-int-) | يضبط إحداثي y للزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| [setYPixel(int value)](#setYPixel-int-) | يضبط إحداثي y للزاوية العلوية اليسرى بوحدات البكسل. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | يضبط إحداثي y للزاوية العلوية اليسرى بوحدات نسبة مساحة المخطط. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyFont() {#applyFont--}
```
public void applyFont()
```


تطبيق الخط الخاص بتسميات البيانات على جميع العقد الفرعية.

### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


يرجع كائن Characters يمثل نطاقًا من الأحرف داخل النص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | int | فهرس بداية الحرف. |
| length | int | عدد الأحرف. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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


يحصل على [getArea()](../../com.aspose.cells/datalabels\#getArea--).

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


يحصل على وضع العرض للخلفية

انظر [BackgroundMode](../../com.aspose.cells/backgroundmode).

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
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


يحصل على اتجاه النص.

انظر [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


يحصل على الخط الخاص بـ DataLabels؛

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


يحصل على ارتفاع الإطار بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. يرجى استخدام الخاصية ChartFrame.HeightRatioToChart بدلاً من ذلك. Height = HeightRatioToChart \* 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ February 2025. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

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


يحصل على ارتفاع الإطار بوحدات نسبة مساحة المخطط.

**Remarks**

هذه قيمة كسرية، النطاق الصالح لها بين 0-1. كيف يمكن تحويل وحدات النسبة إلى بكسل؟ HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### getLinkedSource() {#getLinkedSource--}
```
public String getLinkedSource()
```


يحصل على مرجع إلى ورقة العمل.

**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
```


يحصل على تنسيق الرقم المدمج.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


يمثل سلسلة التنسيق لكائن DataLabels.

**Returns:**
java.lang.String
### getNumberFormatLinked() {#getNumberFormatLinked--}
```
public boolean getNumberFormatLinked()
```


صحيح إذا كان تنسيق الرقم مرتبطًا بالخلايا (بحيث يتغير تنسيق الرقم في التسميات عندما يتغير في الخلايا).

**Returns:**
boolean
### getPosition() {#getPosition--}
```
public int getPosition()
```


يمثل موضع تسمية البيانات.

انظر إلى [LabelPositionType](../../com.aspose.cells/labelpositiontype).

**Returns:**
int
### getReadingOrder() {#getReadingOrder--}
```
public int getReadingOrder()
```


يمثل ترتيب قراءة النص.

انظر [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


يمثل زاوية دوران النص.

**Remarks**


0: غير مدور.

255: من الأعلى إلى الأسفل.

\-90: إلى الأسفل.

90: إلى الأعلى.


**Returns:**
int
### getSeparatorType() {#getSeparatorType--}
```
public int getSeparatorType()
```


يحصل على نوع الفاصل المستخدم لتسميات البيانات في المخطط.

انظر إلى [DataLabelsSeparatorType](../../com.aspose.cells/datalabelsseparatortype).

**Remarks**

لتعيين الفاصل المخصص، يرجى تعيين الخاصية [getSeparatorType()](../../com.aspose.cells/datalabels\#getSeparatorType--) كـ [DataLabelsSeparatorType.CUSTOM](../../com.aspose.cells/datalabelsseparatortype\#CUSTOM) ثم تحديد القيمة المتوقعة لـ [getSeparatorValue()](../../com.aspose.cells/datalabels\#getSeparatorValue--).

**Returns:**
int
### getSeparatorValue() {#getSeparatorValue--}
```
public String getSeparatorValue()
```


يحصل على قيمة الفاصل المستخدمة لتسميات البيانات في المخطط.

**Returns:**
java.lang.String
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
### getShapeType() {#getShapeType--}
```
public int getShapeType()
```


يحصل على نوع الشكل لتسمية البيانات.

انظر إلى [DataLabelShapeType](../../com.aspose.cells/datalabelshapetype).

**Returns:**
int
### getShowBubbleSize() {#getShowBubbleSize--}
```
public boolean getShowBubbleSize()
```


يمثل سلوك عرض قيمة النسبة المئوية لعلامة البيانات في مخطط محدد. True يعرض قيمة النسبة المئوية. False يخفي قيمة النسبة المئوية.

**Returns:**
boolean
### getShowCategoryName() {#getShowCategoryName--}
```
public boolean getShowCategoryName()
```


يمثل سلوك عرض اسم الفئة لعلامة البيانات في مخطط محدد. True لعرض اسم الفئة لعلامات البيانات على المخطط. False لإخفائه.

**Returns:**
boolean
### getShowCellRange() {#getShowCellRange--}
```
public boolean getShowCellRange()
```


يشير إلى ما إذا كان سيتم عرض نطاق الخلايا كتسميات للبيانات.

**Returns:**
boolean
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


يمثل سلوك عرض مفتاح وسيلة الإيضاح لعلامة البيانات في مخطط محدد. True إذا كان مفتاح وسيلة الإيضاح مرئيًا.

**Returns:**
boolean
### getShowPercentage() {#getShowPercentage--}
```
public boolean getShowPercentage()
```


يمثل سلوك عرض قيمة النسبة المئوية لعلامة البيانات في مخطط محدد. True يعرض قيمة النسبة المئوية. False يخفي قيمة النسبة المئوية.

**Returns:**
boolean
### getShowSeriesName() {#getShowSeriesName--}
```
public boolean getShowSeriesName()
```


يشير إلى ما إذا كان اسم السلسلة يُعرض على علامات البيانات في المخطط. True لإظهار اسم السلسلة. False لإخفائه.

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


يمثل سلوك عرض قيم علامة البيانات في مخطط محدد. True يعرض القيم. False يخفيها.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


يحصل على نص تسمية البيانات.

**Remarks**

يعمل فقط عندما تكون هذه علامة بيانات لنقطة مخطط.

**Returns:**
java.lang.String
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


يمثل ترتيب قراءة النص.

انظر [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية ChartTextFrame.ReadingOrder. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2020. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


يحصل على كائن [getFont()](../../com.aspose.cells/chartframe\#getFont--) لكائن ChartFrame المحدد.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية ChartFrame.Font. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2012. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


يحصل على محاذاة النص أفقياً.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


يحصل على خيارات النص.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


يحصل على محاذاة النص عمودياً.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


يحصل على عرض الإطار بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. يرجى استخدام الخاصية ChartFrame.WidthRatioToChart بدلاً من ذلك. Width = WidthRatioToChart \* 4000; سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

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


يحصل على عرض الإطار بوحدات نسبة مساحة المخطط.

**Remarks**

هذه قيمة كسرية، النطاق الصالح لها بين 0-1. كيف يمكن تحويل وحدات النسبة إلى بكسلات؟ WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


يحصل على إحداثي x للزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. يرجى استخدام خاصية ChartFrame.XRatioToChart بدلاً من ذلك. X = XRatioToChart \* 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. شركة Aspose تعتذر عن أي إزعاج قد تكون قد واجهته.

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


يحصل على إحداثي x للزاوية العلوية اليسرى بوحدات نسبة مساحة المخطط.

**Remarks**

هذه قيمة كسرية، النطاق الصالح لها بين 0-1. كيف يتم تحويل وحدات النسبة إلى بكسلات؟ XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


يحصل على إحداثي y للزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. يرجى استخدام خاصية ChartFrame.YRatioToChart بدلاً من ذلك. Y = YRatioToChart \* 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. شركة Aspose تعتذر عن أي إزعاج قد تكون قد واجهته.

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


يحصل على إحداثي y للزاوية العلوية اليسرى بوحدات نسبة مساحة المخطط.

**Remarks**

هذه قيمة كسرية، النطاق الصالح لها بين 0-1. كيف يتم تحويل وحدات النسبة إلى بكسلات؟ YPixel = YRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoText() {#isAutoText--}
```
public boolean isAutoText()
```


يشير إلى أن النص تم إنشاؤه تلقائيًا.

**Returns:**
boolean
### isAutomaticRotation() {#isAutomaticRotation--}
```
public boolean isAutomaticRotation()
```


يشير إلى ما إذا كان نص المخطط يدور تلقائيًا.

**Returns:**
boolean
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
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


يشير إلى ما إذا تم حذف تسمية البيانات هذه.

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
### isNeverOverlap() {#isNeverOverlap--}
```
public boolean isNeverOverlap()
```


يشير إلى ما إذا كانت Datalabels لا تتداخل أبداً عند تحويل مخطط دائري إلى صورة. ملاحظة: هذه الخاصية ذات معنى فقط عند تحويل مخطط دائري إلى صورة.

**Returns:**
boolean
### isResizeShapeToFitText() {#isResizeShapeToFitText--}
```
public boolean isResizeShapeToFitText()
```


يحصل على ما إذا كان يجب أن يتناسب الشكل تلقائيًا لاحتواء النص الموصوف بداخله بالكامل. التناسب التلقائي هو عندما يتم تحجيم النص داخل الشكل لاحتواء جميع النص داخل الشكل.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


يحصل على قيمة تشير إلى ما إذا كان النص مُلتفًا.

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

### setAutoText(boolean value) {#setAutoText-boolean-}
```
public void setAutoText(boolean value)
```


يشير إلى أن النص تم إنشاؤه تلقائيًا.

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


يضبط وضع العرض للخلفية

انظر [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


يشير إلى ما إذا تم حذف تسمية البيانات هذه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDirectionType(int value) {#setDirectionType-int-}
```
public void setDirectionType(int value)
```


يضبط اتجاه النص.

انظر [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


يضبط ارتفاع الإطار بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. يرجى استخدام الخاصية ChartFrame.HeightRatioToChart بدلاً من ذلك. Height = HeightRatioToChart \* 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ February 2025. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

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


يضبط ارتفاع الإطار بوحدات نسبة مساحة المخطط.

**Remarks**

هذه قيمة كسرية، النطاق الصالح لها بين 0-1. كيف يمكن تحويل وحدات النسبة إلى بكسل؟ HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

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

### setLinkedSource(String value) {#setLinkedSource-java.lang.String-}
```
public void setLinkedSource(String value)
```


يضبط مرجعًا إلى ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setNeverOverlap(boolean value) {#setNeverOverlap-boolean-}
```
public void setNeverOverlap(boolean value)
```


يشير إلى ما إذا كانت Datalabels لا تتداخل أبداً عند تحويل مخطط دائري إلى صورة. ملاحظة: هذه الخاصية ذات معنى فقط عند تحويل مخطط دائري إلى صورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


يضبط تنسيق الرقم المدمج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


يمثل سلسلة التنسيق لكائن DataLabels.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setNumberFormatLinked(boolean value) {#setNumberFormatLinked-boolean-}
```
public void setNumberFormatLinked(boolean value)
```


صحيح إذا كان تنسيق الرقم مرتبطًا بالخلايا (بحيث يتغير تنسيق الرقم في التسميات عندما يتغير في الخلايا).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


يمثل موضع تسمية البيانات.

انظر إلى [LabelPositionType](../../com.aspose.cells/labelpositiontype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


ضبط موضع الإطار إلى تلقائي

### setReadingOrder(int value) {#setReadingOrder-int-}
```
public void setReadingOrder(int value)
```


يمثل ترتيب قراءة النص.

انظر [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setResizeShapeToFitText(boolean value) {#setResizeShapeToFitText-boolean-}
```
public void setResizeShapeToFitText(boolean value)
```


يضبط ما إذا كان يجب أن يتناسب الشكل تلقائيًا لاحتواء النص الموصوف بداخله بالكامل. التناسب التلقائي هو عندما يتم تحجيم النص داخل الشكل لاحتواء جميع النص داخل الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


يمثل زاوية دوران النص.

**Remarks**


0: غير مدور.

255: من الأعلى إلى الأسفل.

\-90: إلى الأسفل.

90: إلى الأعلى.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSeparatorType(int value) {#setSeparatorType-int-}
```
public void setSeparatorType(int value)
```


يضبط نوع الفاصل المستخدم لتسميات البيانات في المخطط.

انظر إلى [DataLabelsSeparatorType](../../com.aspose.cells/datalabelsseparatortype).

**Remarks**

لتعيين الفاصل المخصص، يرجى تعيين الخاصية [getSeparatorType()](../../com.aspose.cells/datalabels\#getSeparatorType--) كـ [DataLabelsSeparatorType.CUSTOM](../../com.aspose.cells/datalabelsseparatortype\#CUSTOM) ثم تحديد القيمة المتوقعة لـ [getSeparatorValue()](../../com.aspose.cells/datalabels\#getSeparatorValue--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSeparatorValue(String value) {#setSeparatorValue-java.lang.String-}
```
public void setSeparatorValue(String value)
```


يضبط قيمة الفاصل المستخدمة لتسميات البيانات في المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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

### setShapeType(int value) {#setShapeType-int-}
```
public void setShapeType(int value)
```


يضبط نوع الشكل لتسمية البيانات.

انظر إلى [DataLabelShapeType](../../com.aspose.cells/datalabelshapetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setShowBubbleSize(boolean value) {#setShowBubbleSize-boolean-}
```
public void setShowBubbleSize(boolean value)
```


يمثل سلوك عرض قيمة النسبة المئوية لعلامة البيانات في مخطط محدد. True يعرض قيمة النسبة المئوية. False يخفي قيمة النسبة المئوية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowCategoryName(boolean value) {#setShowCategoryName-boolean-}
```
public void setShowCategoryName(boolean value)
```


يمثل سلوك عرض اسم الفئة لعلامة البيانات في مخطط محدد. True لعرض اسم الفئة لعلامات البيانات على المخطط. False لإخفائه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowCellRange(boolean value) {#setShowCellRange-boolean-}
```
public void setShowCellRange(boolean value)
```


يشير إلى ما إذا كان سيتم عرض نطاق الخلايا كتسميات للبيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


يمثل سلوك عرض مفتاح وسيلة الإيضاح لعلامة البيانات في مخطط محدد. True إذا كان مفتاح وسيلة الإيضاح مرئيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowPercentage(boolean value) {#setShowPercentage-boolean-}
```
public void setShowPercentage(boolean value)
```


يمثل سلوك عرض قيمة النسبة المئوية لعلامة البيانات في مخطط محدد. True يعرض قيمة النسبة المئوية. False يخفي قيمة النسبة المئوية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowSeriesName(boolean value) {#setShowSeriesName-boolean-}
```
public void setShowSeriesName(boolean value)
```


يشير إلى ما إذا كان اسم السلسلة يُعرض على علامات البيانات في المخطط. True لإظهار اسم السلسلة. False لإخفائه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


يمثل سلوك عرض قيم علامة البيانات في مخطط محدد. True يعرض القيم. False يخفيها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


يضبط نص تسمية البيانات.

**Remarks**

يعمل فقط عندما تكون هذه علامة بيانات لنقطة مخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


يمثل ترتيب قراءة النص.

انظر [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية ChartTextFrame.ReadingOrder. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2020. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


يضبط محاذاة النص أفقياً.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


يضبط محاذاة النص عموديًا.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان النص مُلتفًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


يضبط عرض الإطار بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. يرجى استخدام الخاصية ChartFrame.WidthRatioToChart بدلاً من ذلك. Width = WidthRatioToChart \* 4000; سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

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


يضبط عرض الإطار بوحدات نسبة مساحة المخطط.

**Remarks**

هذه قيمة كسرية، النطاق الصالح لها بين 0-1. كيف يمكن تحويل وحدات النسبة إلى بكسلات؟ WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


يضبط إحداثي x للزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. يرجى استخدام خاصية ChartFrame.XRatioToChart بدلاً من ذلك. X = XRatioToChart \* 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. شركة Aspose تعتذر عن أي إزعاج قد تكون قد واجهته.

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


يضبط إحداثي x للزاوية العلوية اليسرى بوحدات نسبة مساحة المخطط.

**Remarks**

هذه قيمة كسرية، النطاق الصالح لها بين 0-1. كيف يتم تحويل وحدات النسبة إلى بكسلات؟ XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


يضبط إحداثي y للزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. يرجى استخدام خاصية ChartFrame.YRatioToChart بدلاً من ذلك. Y = YRatioToChart \* 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. شركة Aspose تعتذر عن أي إزعاج قد تكون قد واجهته.

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


يضبط إحداثي y للزاوية العلوية اليسرى بوحدات نسبة مساحة المخطط.

**Remarks**

هذه قيمة كسرية، النطاق الصالح لها بين 0-1. كيف يتم تحويل وحدات النسبة إلى بكسلات؟ YPixel = YRatioToChart \* Chart.ChartObject.Height;

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

