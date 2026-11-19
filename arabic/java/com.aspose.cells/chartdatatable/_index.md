---
title: "ChartDataTable"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل جدول بيانات المخطط."
type: docs
url: /ar/java/com.aspose.cells/chartdatatable/
---

**Inheritance:**
java.lang.Object
```
public class ChartDataTable
```

يمثل جدول بيانات المخطط.

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
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 10);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         chart.setShowDataTable(true);
 
         //Getting Chart Table
         ChartDataTable chartTable = chart.getChartDataTable();
 
         //Setting Chart Table Font Color
         chartTable.getFont().setColor(com.aspose.cells.Color.getRed());
 
         //Setting Legend Key VisibilityOptions
         chartTable.setShowLegendKey(false);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoScaleFont()](#getAutoScaleFont--) | صحيح إذا كان النص داخل الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. |
| [getBackgroundMode()](#getBackgroundMode--) | يحصل على وضع العرض للخلفية |
| [getBorder()](#getBorder--) | يرجع كائن Border الذي يمثل حد الكائن. |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | يحصل على كائن [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) الذي يمثل إعداد الخط لجدول البيانات المخطط المحدد. |
| [getShowLegendKey()](#getShowLegendKey--) | صحيح إذا كان مفتاح وسيلة إيضاح تسمية البيانات مرئيًا. |
| [hasBorderHorizontal()](#hasBorderHorizontal--) | صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا أفقية |
| [hasBorderOutline()](#hasBorderOutline--) | صحيح إذا كان جدول بيانات المخطط يحتوي على حدود المخطط |
| [hasBorderVertical()](#hasBorderVertical--) | صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا عمودية |
| [hasHorizontalBorder()](#hasHorizontalBorder--) | صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا أفقية |
| [hasOutlineBorder()](#hasOutlineBorder--) | صحيح إذا كان جدول بيانات المخطط يحتوي على حدود المخطط |
| [hasVerticalBorder()](#hasVerticalBorder--) | صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا عمودية |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | صحيح إذا كان النص داخل الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | يضبط وضع العرض للخلفية |
| [setHasBorderHorizontal(boolean value)](#setHasBorderHorizontal-boolean-) | صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا أفقية |
| [setHasBorderOutline(boolean value)](#setHasBorderOutline-boolean-) | صحيح إذا كان جدول بيانات المخطط يحتوي على حدود المخطط |
| [setHasBorderVertical(boolean value)](#setHasBorderVertical-boolean-) | صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا عمودية |
| [setHasHorizontalBorder(boolean value)](#setHasHorizontalBorder-boolean-) | صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا أفقية |
| [setHasOutlineBorder(boolean value)](#setHasOutlineBorder-boolean-) | صحيح إذا كان جدول بيانات المخطط يحتوي على حدود المخطط |
| [setHasVerticalBorder(boolean value)](#setHasVerticalBorder-boolean-) | صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا عمودية |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | صحيح إذا كان مفتاح وسيلة إيضاح تسمية البيانات مرئيًا. |
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
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


صحيح إذا كان النص داخل الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. القيمة الافتراضية هي صحيح.

**Returns:**
boolean
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


يرجع كائن Border الذي يمثل حد الكائن.

**Returns:**
[Line](../../com.aspose.cells/line)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public Font getFont()
```


يحصل على كائن [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) الذي يمثل إعداد الخط لجدول البيانات المخطط المحدد.

**Returns:**
[Font](../../com.aspose.cells/font)
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


صحيح إذا كان مفتاح وسيلة إيضاح تسمية البيانات مرئيًا.

**Returns:**
boolean
### hasBorderHorizontal() {#hasBorderHorizontal--}
```
public boolean hasBorderHorizontal()
```


صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا أفقية

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ChartDataTable.HasHorizontalBorder. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### hasBorderOutline() {#hasBorderOutline--}
```
public boolean hasBorderOutline()
```


صحيح إذا كان جدول بيانات المخطط يحتوي على حدود المخطط

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ChartDataTable.HasOutlineBorder. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### hasBorderVertical() {#hasBorderVertical--}
```
public boolean hasBorderVertical()
```


صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا عمودية

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ChartDataTable.HasVerticalBorder. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### hasHorizontalBorder() {#hasHorizontalBorder--}
```
public boolean hasHorizontalBorder()
```


صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا أفقية

**Returns:**
boolean
### hasOutlineBorder() {#hasOutlineBorder--}
```
public boolean hasOutlineBorder()
```


صحيح إذا كان جدول بيانات المخطط يحتوي على حدود المخطط

**Returns:**
boolean
### hasVerticalBorder() {#hasVerticalBorder--}
```
public boolean hasVerticalBorder()
```


صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا عمودية

**Returns:**
boolean
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




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


صحيح إذا كان النص داخل الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. القيمة الافتراضية هي صحيح.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

### setHasBorderHorizontal(boolean value) {#setHasBorderHorizontal-boolean-}
```
public void setHasBorderHorizontal(boolean value)
```


صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا أفقية

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ChartDataTable.HasHorizontalBorder. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasBorderOutline(boolean value) {#setHasBorderOutline-boolean-}
```
public void setHasBorderOutline(boolean value)
```


صحيح إذا كان جدول بيانات المخطط يحتوي على حدود المخطط

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ChartDataTable.HasOutlineBorder. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasBorderVertical(boolean value) {#setHasBorderVertical-boolean-}
```
public void setHasBorderVertical(boolean value)
```


صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا عمودية

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ChartDataTable.HasVerticalBorder. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasHorizontalBorder(boolean value) {#setHasHorizontalBorder-boolean-}
```
public void setHasHorizontalBorder(boolean value)
```


صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا أفقية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasOutlineBorder(boolean value) {#setHasOutlineBorder-boolean-}
```
public void setHasOutlineBorder(boolean value)
```


صحيح إذا كان جدول بيانات المخطط يحتوي على حدود المخطط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasVerticalBorder(boolean value) {#setHasVerticalBorder-boolean-}
```
public void setHasVerticalBorder(boolean value)
```


صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا عمودية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


صحيح إذا كان مفتاح وسيلة إيضاح تسمية البيانات مرئيًا.

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

