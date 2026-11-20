---
title: "ChartDataTable"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет таблицу данных диаграммы."
type: docs
url: /ru/java/com.aspose.cells/chartdatatable/
---

**Inheritance:**
java.lang.Object
```
public class ChartDataTable
```

Представляет таблицу данных диаграммы.

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
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoScaleFont()](#getAutoScaleFont--) | True, если текст в объекте изменяет размер шрифта при изменении размера объекта. |
| [getBackgroundMode()](#getBackgroundMode--) | Получает режим отображения фона |
| [getBorder()](#getBorder--) | Возвращает объект Border, который представляет границу объекта. |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Получает объект [getFont()](../../com.aspose.cells/chartdatatable\#getFont--), который представляет настройки шрифта указанной таблицы данных диаграммы. |
| [getShowLegendKey()](#getShowLegendKey--) | True, если ключ легенды подписи данных виден. |
| [hasBorderHorizontal()](#hasBorderHorizontal--) | True, если у таблицы данных диаграммы есть горизонтальные границы ячеек. |
| [hasBorderOutline()](#hasBorderOutline--) | True, если у таблицы данных диаграммы есть контурные границы. |
| [hasBorderVertical()](#hasBorderVertical--) | True, если у таблицы данных диаграммы есть вертикальные границы ячеек. |
| [hasHorizontalBorder()](#hasHorizontalBorder--) | True, если у таблицы данных диаграммы есть горизонтальные границы ячеек. |
| [hasOutlineBorder()](#hasOutlineBorder--) | True, если у таблицы данных диаграммы есть контурные границы. |
| [hasVerticalBorder()](#hasVerticalBorder--) | True, если у таблицы данных диаграммы есть вертикальные границы ячеек. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | True, если текст в объекте изменяет размер шрифта при изменении размера объекта. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Устанавливает режим отображения фона |
| [setHasBorderHorizontal(boolean value)](#setHasBorderHorizontal-boolean-) | True, если у таблицы данных диаграммы есть горизонтальные границы ячеек. |
| [setHasBorderOutline(boolean value)](#setHasBorderOutline-boolean-) | True, если у таблицы данных диаграммы есть контурные границы. |
| [setHasBorderVertical(boolean value)](#setHasBorderVertical-boolean-) | True, если у таблицы данных диаграммы есть вертикальные границы ячеек. |
| [setHasHorizontalBorder(boolean value)](#setHasHorizontalBorder-boolean-) | True, если у таблицы данных диаграммы есть горизонтальные границы ячеек. |
| [setHasOutlineBorder(boolean value)](#setHasOutlineBorder-boolean-) | True, если у таблицы данных диаграммы есть контурные границы. |
| [setHasVerticalBorder(boolean value)](#setHasVerticalBorder-boolean-) | True, если у таблицы данных диаграммы есть вертикальные границы ячеек. |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | True, если ключ легенды подписи данных виден. |
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
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


True, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию — True.

**Returns:**
boolean
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Получает режим отображения фона

Смотрите [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Возвращает объект Border, который представляет границу объекта.

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


Получает объект [getFont()](../../com.aspose.cells/chartdatatable\#getFont--), который представляет настройки шрифта указанной таблицы данных диаграммы.

**Returns:**
[Font](../../com.aspose.cells/font)
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


True, если ключ легенды подписи данных виден.

**Returns:**
boolean
### hasBorderHorizontal() {#hasBorderHorizontal--}
```
public boolean hasBorderHorizontal()
```


True, если у таблицы данных диаграммы есть горизонтальные границы ячеек.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство ChartDataTable.HasHorizontalBorder. Это свойство будет удалено через 12 месяцев, начиная с июня 2024 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### hasBorderOutline() {#hasBorderOutline--}
```
public boolean hasBorderOutline()
```


True, если у таблицы данных диаграммы есть контурные границы.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство ChartDataTable.HasOutlineBorder. Это свойство будет удалено через 12 месяцев, начиная с июня 2024 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### hasBorderVertical() {#hasBorderVertical--}
```
public boolean hasBorderVertical()
```


True, если у таблицы данных диаграммы есть вертикальные границы ячеек.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство ChartDataTable.HasVerticalBorder. Это свойство будет удалено через 12 месяцев, начиная с июня 2024 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### hasHorizontalBorder() {#hasHorizontalBorder--}
```
public boolean hasHorizontalBorder()
```


True, если у таблицы данных диаграммы есть горизонтальные границы ячеек.

**Returns:**
boolean
### hasOutlineBorder() {#hasOutlineBorder--}
```
public boolean hasOutlineBorder()
```


True, если у таблицы данных диаграммы есть контурные границы.

**Returns:**
boolean
### hasVerticalBorder() {#hasVerticalBorder--}
```
public boolean hasVerticalBorder()
```


True, если у таблицы данных диаграммы есть вертикальные границы ячеек.

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


True, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию — True.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Устанавливает режим отображения фона

Смотрите [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHasBorderHorizontal(boolean value) {#setHasBorderHorizontal-boolean-}
```
public void setHasBorderHorizontal(boolean value)
```


True, если у таблицы данных диаграммы есть горизонтальные границы ячеек.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство ChartDataTable.HasHorizontalBorder. Это свойство будет удалено через 12 месяцев, начиная с июня 2024 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasBorderOutline(boolean value) {#setHasBorderOutline-boolean-}
```
public void setHasBorderOutline(boolean value)
```


True, если у таблицы данных диаграммы есть контурные границы.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство ChartDataTable.HasOutlineBorder. Это свойство будет удалено через 12 месяцев, начиная с июня 2024 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasBorderVertical(boolean value) {#setHasBorderVertical-boolean-}
```
public void setHasBorderVertical(boolean value)
```


True, если у таблицы данных диаграммы есть вертикальные границы ячеек.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство ChartDataTable.HasVerticalBorder. Это свойство будет удалено через 12 месяцев, начиная с июня 2024 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasHorizontalBorder(boolean value) {#setHasHorizontalBorder-boolean-}
```
public void setHasHorizontalBorder(boolean value)
```


True, если у таблицы данных диаграммы есть горизонтальные границы ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasOutlineBorder(boolean value) {#setHasOutlineBorder-boolean-}
```
public void setHasOutlineBorder(boolean value)
```


True, если у таблицы данных диаграммы есть контурные границы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasVerticalBorder(boolean value) {#setHasVerticalBorder-boolean-}
```
public void setHasVerticalBorder(boolean value)
```


True, если у таблицы данных диаграммы есть вертикальные границы ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


True, если ключ легенды подписи данных виден.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

