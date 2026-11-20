---
title: "Область"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий формат области."
type: docs
url: /ru/java/com.aspose.cells/area/
---

**Inheritance:**
java.lang.Object
```
public class Area
```

Инкапсулирует объект, представляющий формат области.

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
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundColor()](#getBackgroundColor--) | Получает фоновый [Color](../../com.aspose.cells/color) области [Area](../../com.aspose.cells/area). |
| [getClass()](#getClass--) |  |
| [getFillFormat()](#getFillFormat--) | Представляет объект [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--), который содержит свойства заливки для указанной диаграммы или фигуры. |
| [getForegroundColor()](#getForegroundColor--) | Получает передний [Color](../../com.aspose.cells/color). |
| [getFormatting()](#getFormatting--) | Представляет форматирование области. |
| [getInvertIfNegative()](#getInvertIfNegative--) | Если свойство истинно и значение точки диаграммы является отрицательным числом, цвета переднего плана и фона будут обменены. |
| [getTransparency()](#getTransparency--) | Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | Устанавливает фоновый [Color](../../com.aspose.cells/color) области [Area](../../com.aspose.cells/area). |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | Устанавливает передний [Color](../../com.aspose.cells/color). |
| [setFormatting(int value)](#setFormatting-int-) | Представляет форматирование области. |
| [setInvertIfNegative(boolean value)](#setInvertIfNegative-boolean-) | Если свойство истинно и значение точки диаграммы является отрицательным числом, цвета переднего плана и фона будут обменены. |
| [setTransparency(double value)](#setTransparency-double-) | Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Получает фоновый [Color](../../com.aspose.cells/color) области [Area](../../com.aspose.cells/area).

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


Представляет объект [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--), который содержит свойства заливки для указанной диаграммы или фигуры.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


Получает передний [Color](../../com.aspose.cells/color).

**Returns:**
[Color](../../com.aspose.cells/color)
### getFormatting() {#getFormatting--}
```
public int getFormatting()
```


Представляет форматирование области.

Смотрите [FormattingType](../../com.aspose.cells/formattingtype).

**Returns:**
int
### getInvertIfNegative() {#getInvertIfNegative--}
```
public boolean getInvertIfNegative()
```


Если свойство истинно и значение точки диаграммы является отрицательным числом, цвета переднего плана и фона будут обменены.

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


Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный).

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


Устанавливает фоновый [Color](../../com.aspose.cells/color) области [Area](../../com.aspose.cells/area).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


Устанавливает передний [Color](../../com.aspose.cells/color).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setFormatting(int value) {#setFormatting-int-}
```
public void setFormatting(int value)
```


Представляет форматирование области.

Смотрите [FormattingType](../../com.aspose.cells/formattingtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setInvertIfNegative(boolean value) {#setInvertIfNegative-boolean-}
```
public void setInvertIfNegative(boolean value)
```


Если свойство истинно и значение точки диаграммы является отрицательным числом, цвета переднего плана и фона будут обменены.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

