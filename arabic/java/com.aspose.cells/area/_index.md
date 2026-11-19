---
title: "منطقة"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على الكائن الذي يمثل تنسيق المنطقة."
type: docs
url: /ar/java/com.aspose.cells/area/
---

**Inheritance:**
java.lang.Object
```
public class Area
```

يحتوي على الكائن الذي يمثل تنسيق المنطقة.

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
         //Setting the foreground color of the plot area
         chart.getPlotArea().getArea().setForegroundColor(Color.getBlue()); //Blue
         //Setting the foreground color of the chart area
         chart.getChartArea().getArea().setForegroundColor(Color.getYellow()); //Yellow
         //Setting the foreground color of the 1st NSeries area
         chart.getNSeries().get(0).getArea().setForegroundColor(Color.getRed()); //Red
         //Setting the foreground color of the area of the 1st NSeries point
         chart.getNSeries().get(0).getPoints().get(0).getArea().setForegroundColor(Color.getCyan()); //Cyan
         //Saving the Excel file
         workbook.save("book1.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundColor()](#getBackgroundColor--) | يحصل على [Color](../../com.aspose.cells/color) الخلفية للـ[Area](../../com.aspose.cells/area). |
| [getClass()](#getClass--) |  |
| [getFillFormat()](#getFillFormat--) | يمثل كائنًا [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) يحتوي على خصائص تنسيق التعبئة للمخطط أو الشكل المحدد. |
| [getForegroundColor()](#getForegroundColor--) | يحصل على [Color](../../com.aspose.cells/color) في المقدمة. |
| [getFormatting()](#getFormatting--) | يمثل تنسيق المنطقة. |
| [getInvertIfNegative()](#getInvertIfNegative--) | إذا كانت الخاصية true وكانت قيمة نقطة المخطط رقمًا سالبًا، سيتم تبادل لون المقدمة ولون الخلفية. |
| [getTransparency()](#getTransparency--) | يرجع أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | يضبط [Color](../../com.aspose.cells/color) الخلفية للـ[Area](../../com.aspose.cells/area). |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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

