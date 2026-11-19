---
title: "الجدران"
second_title: "Aspose.Cells for Java API Reference"
description: "يغلف الكائن الذي يمثل جدران مخطط ثلاثي الأبعاد."
type: docs
url: /ar/java/com.aspose.cells/walls/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Area](../../com.aspose.cells/area), [com.aspose.cells.Floor](../../com.aspose.cells/floor)
```
public class Walls extends Floor
```

يغلف الكائن الذي يمثل جدران مخطط ثلاثي الأبعاد.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundColor()](#getBackgroundColor--) | يحصل على [Color](../../com.aspose.cells/color) الخلفية للـ[Area](../../com.aspose.cells/area). |
| [getBorder()](#getBorder--) | يحصل على الحد [Line](../../com.aspose.cells/line). |
| [getCenterX()](#getCenterX--) | يحصل على إحداثي x للزاوية اليسرى السفلية لمركز الجدار بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [getCenterXPx()](#getCenterXPx--) | يحصل على إحداثي x للزاوية اليسرى السفلية لمركز الجدار بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [getCenterY()](#getCenterY--) | يحصل على إحداثي y للزاوية اليسرى السفلية لمركز الجدار بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [getCenterYPx()](#getCenterYPx--) | يحصل على إحداثي y للزاوية اليسرى السفلية لمركز الجدار بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [getClass()](#getClass--) |  |
| [getCubePointCount()](#getCubePointCount--) | يحصل على عدد نقاط المكعب بعد استدعاء طريقة Chart.Calculate(). |
| [getCubePointXPx(int index)](#getCubePointXPx-int-) | يحصل على إحداثي x لنقطة القمة لمكعب الجدران بعد استدعاء طريقة Chart.Calculate(). |
| [getCubePointYPx(int index)](#getCubePointYPx-int-) | يحصل على إحداثي y لنقطة القمة لمكعب الجدران بعد استدعاء طريقة Chart.Calculate(). |
| [getDepth()](#getDepth--) | يحصل على العمق من الأمام إلى الخلف بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [getDepthPx()](#getDepthPx--) | يحصل على العمق من الأمام إلى الخلف بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [getFillFormat()](#getFillFormat--) | يمثل كائنًا [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) يحتوي على خصائص تنسيق التعبئة للمخطط أو الشكل المحدد. |
| [getForegroundColor()](#getForegroundColor--) | يحصل على [Color](../../com.aspose.cells/color) في المقدمة. |
| [getFormatting()](#getFormatting--) | يمثل تنسيق المنطقة. |
| [getHeight()](#getHeight--) | يحصل على الارتفاع من الأعلى إلى الأسفل بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [getHeightPx()](#getHeightPx--) | يحصل على الارتفاع من الأعلى إلى الأسفل بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [getInvertIfNegative()](#getInvertIfNegative--) | إذا كانت الخاصية true وكانت قيمة نقطة المخطط رقمًا سالبًا، سيتم تبادل لون المقدمة ولون الخلفية. |
| [getTransparency()](#getTransparency--) | يرجع أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [getWidth()](#getWidth--) | يحصل على العرض من اليسار إلى اليمين بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [getWidthPx()](#getWidthPx--) | يحصل على العرض من اليسار إلى اليمين بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | يضبط [Color](../../com.aspose.cells/color) الخلفية للـ[Area](../../com.aspose.cells/area). |
| [setBorder(Line value)](#setBorder-com.aspose.cells.Line-) | يضبط الحد [Line](../../com.aspose.cells/line). |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | يضبط [Color](../../com.aspose.cells/color) في المقدمة. |
| [setFormatting(int value)](#setFormatting-int-) | يمثل تنسيق المنطقة. |
| [setInvertIfNegative(boolean value)](#setInvertIfNegative-boolean-) | إذا كانت الخاصية true وكانت قيمة نقطة المخطط رقمًا سالبًا، سيتم تبادل لون المقدمة ولون الخلفية. |
| [setTransparency(double value)](#setTransparency-double-) | يرجع أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
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
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


يحصل على [Color](../../com.aspose.cells/color) الخلفية للـ[Area](../../com.aspose.cells/area).

**Returns:**
[Color](../../com.aspose.cells/color)
### getBorder() {#getBorder--}
```
public Line getBorder()
```


يحصل على الحد [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getCenterX() {#getCenterX--}
```
public int getCenterX()
```


يحصل على إحداثي x للزاوية اليسرى السفلية لمركز الجدار بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getCenterXPx() {#getCenterXPx--}
```
public int getCenterXPx()
```


يحصل على إحداثي x للزاوية اليسرى السفلية لمركز الجدار بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getCenterY() {#getCenterY--}
```
public int getCenterY()
```


يحصل على إحداثي y للزاوية اليسرى السفلية لمركز الجدار بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getCenterYPx() {#getCenterYPx--}
```
public int getCenterYPx()
```


يحصل على إحداثي y للزاوية اليسرى السفلية لمركز الجدار بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCubePointCount() {#getCubePointCount--}
```
public int getCubePointCount()
```


يحصل على عدد نقاط المكعب بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getCubePointXPx(int index) {#getCubePointXPx-int-}
```
public float getCubePointXPx(int index)
```


يحصل على إحداثي x لنقطة القمة لمكعب الجدران بعد استدعاء طريقة Chart.Calculate(). عدد نقاط القمة لمكعب الجدران هو ثمانية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
float
### getCubePointYPx(int index) {#getCubePointYPx-int-}
```
public float getCubePointYPx(int index)
```


يحصل على إحداثي y لنقطة القمة لمكعب الجدران بعد استدعاء طريقة Chart.Calculate(). عدد نقاط القمة لمكعب الجدران هو ثمانية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
float
### getDepth() {#getDepth--}
```
public int getDepth()
```


يحصل على العمق من الأمام إلى الخلف بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getDepthPx() {#getDepthPx--}
```
public int getDepthPx()
```


يحصل على العمق من الأمام إلى الخلف بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getFillFormat() {#getFillFormat--}
```
public FillFormat getFillFormat()
```


يمثل كائنًا [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) يحتوي على خصائص تنسيق التعبئة للمخطط أو الشكل المحدد.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


يحصل على [Color](../../com.aspose.cells/color) في المقدمة.

**Returns:**
[Color](../../com.aspose.cells/color)
### getFormatting() {#getFormatting--}
```
public int getFormatting()
```


يمثل تنسيق المنطقة.

انظر [FormattingType](../../com.aspose.cells/formattingtype).

**Returns:**
int
### getHeight() {#getHeight--}
```
public int getHeight()
```


يحصل على الارتفاع من الأعلى إلى الأسفل بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getHeightPx() {#getHeightPx--}
```
public int getHeightPx()
```


يحصل على الارتفاع من الأعلى إلى الأسفل بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getInvertIfNegative() {#getInvertIfNegative--}
```
public boolean getInvertIfNegative()
```


إذا كانت الخاصية true وكانت قيمة نقطة المخطط رقمًا سالبًا، سيتم تبادل لون المقدمة ولون الخلفية.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Workbook object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(-100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "A3"
         chart.getNSeries().add("A1:A3", true);
         boolean isNegative = chart.getNSeries().get(0).getArea().getInvertIfNegative();
         chart.getNSeries().get(0).getArea().setInvertIfNegative(true);
         //Setting the foreground color of the 1st NSeries area
         chart.getNSeries().get(0).getArea().setForegroundColor(Color.getRed());
         //Setting the background color of the 1st NSeries area.
         //The displayed area color of second chart point will be the background color.
         chart.getNSeries().get(0).getArea().setBackgroundColor(Color.getYellow());
         //Saving the Excel file
         workbook.save("book1.xls");
```

**Returns:**
boolean
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


يرجع أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

**Returns:**
double
### getWidth() {#getWidth--}
```
public int getWidth()
```


يحصل على العرض من اليسار إلى اليمين بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate().

**Returns:**
int
### getWidthPx() {#getWidthPx--}
```
public int getWidthPx()
```


يحصل على العرض من اليسار إلى اليمين بوحدات البكسل بعد استدعاء طريقة Chart.Calculate().

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




### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```


يضبط [Color](../../com.aspose.cells/color) الخلفية للـ[Area](../../com.aspose.cells/area).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setBorder(Line value) {#setBorder-com.aspose.cells.Line-}
```
public void setBorder(Line value)
```


يضبط الحد [Line](../../com.aspose.cells/line).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Line](../../com.aspose.cells/line) |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


يضبط [Color](../../com.aspose.cells/color) في المقدمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setFormatting(int value) {#setFormatting-int-}
```
public void setFormatting(int value)
```


يمثل تنسيق المنطقة.

انظر [FormattingType](../../com.aspose.cells/formattingtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setInvertIfNegative(boolean value) {#setInvertIfNegative-boolean-}
```
public void setInvertIfNegative(boolean value)
```


إذا كانت الخاصية true وكانت قيمة نقطة المخطط رقمًا سالبًا، سيتم تبادل لون المقدمة ولون الخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


يرجع أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

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

