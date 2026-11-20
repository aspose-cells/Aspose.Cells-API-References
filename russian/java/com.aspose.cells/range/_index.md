---
title: "Range"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий диапазон ячеек в электронной таблице."
type: docs
url: /ru/java/com.aspose.cells/range/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Range implements Iterable
```

Инкапсулирует объект, представляющий диапазон ячеек в электронной таблице.

**Remarks**

Класс Range обозначает область листа Excel. С его помощью вы можете форматировать и задавать значение диапазона. И вы также можете просто копировать диапазон Excel.

**Example**

В следующем примере показано, как создать диапазон и задать значение диапазону Excel.

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         // Create a range (A1:D3).
         Range range = cells.createRange("A1", "D3");
         // Set value to the range.
         range.setValue("Hello");
         //Save the Excel file
         workbook.save("book1.xlsm");
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Range(CellArea ca, Cells cells)](#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-) | Конструктор класса. |
| [Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)](#Range-int-int-int-int-com.aspose.cells.Cells-) | Конструктор класса. |
## Методы

| Метод | Описание |
| --- | --- |
| [addHyperlink(String address, String textToDisplay, String screenTip)](#addHyperlink-java.lang.String-java.lang.String-java.lang.String-) | Добавляет гиперссылку в указанную ячейку или диапазон ячеек. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Применяет форматы ко всему диапазону. |
| [autoFill(Range target)](#autoFill-com.aspose.cells.Range-) | Автоматически заполняет целевой диапазон. |
| [autoFill(Range target, int autoFillType)](#autoFill-com.aspose.cells.Range-int-) | Автоматически заполняет целевой диапазон. |
| [clear()](#clear--) | Очищает этот диапазон. |
| [clearComments()](#clearComments--) | Очищает комментарии этого диапазона. |
| [clearContents()](#clearContents--) | Очищает содержимое этого диапазона. |
| [clearFormats()](#clearFormats--) | Очищает форматы этого диапазона. |
| [clearHyperlinks(boolean clearFormat)](#clearHyperlinks-boolean-) | Только удаляет гиперссылки. |
| [copy(Range range)](#copy-com.aspose.cells.Range-) | Копирует данные (включая формулы), форматирование, графические объекты и т.д. из исходного диапазона. |
| [copy(Range range, PasteOptions options)](#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-) | Копирование диапазона с параметрами «Специальная вставка». |
| [copyData(Range range)](#copyData-com.aspose.cells.Range-) | Копирует данные ячеек (включая формулы) из исходного диапазона. |
| [copyStyle(Range range)](#copyStyle-com.aspose.cells.Range-) | Копирует настройки стиля из исходного диапазона. |
| [copyValue(Range range)](#copyValue-com.aspose.cells.Range-) | Копирует значение ячейки из исходного диапазона. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowOffset, int columnOffset)](#get-int-int-) | Получает объект [Cell](../../com.aspose.cells/cell) в этом диапазоне. |
| [getAddress()](#getAddress--) | Получает адрес диапазона. |
| [getCellOrNull(int rowOffset, int columnOffset)](#getCellOrNull-int-int-) | Получает объект [Cell](../../com.aspose.cells/cell) или null в этом диапазоне. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Получает количество столбцов в диапазоне. |
| [getColumnWidth()](#getColumnWidth--) | Устанавливает или получает ширину столбца этого диапазона |
| [getCurrentRegion()](#getCurrentRegion--) | Возвращает объект Range, представляющий текущий регион. |
| [getEntireColumn()](#getEntireColumn--) | Получает объект Range, представляющий весь столбец (или столбцы), содержащий указанный диапазон. |
| [getEntireRow()](#getEntireRow--) | Получает объект Range, представляющий всю строку (или строки), содержащую указанный диапазон. |
| [getFirstColumn()](#getFirstColumn--) | Получает индекс первого столбца диапазона. |
| [getFirstRow()](#getFirstRow--) | Получает индекс первой строки диапазона. |
| [getHeight()](#getHeight--) | Получает ширину диапазона в пунктах. |
| [getHyperlinks()](#getHyperlinks--) | Получает все гиперссылки в диапазоне. |
| [getLeft()](#getLeft--) | Получает расстояние в пунктах от левого края столбца A до левого края диапазона. |
| [getName()](#getName--) | Получает имя диапазона. |
| [getOffset(int rowOffset, int columnOffset)](#getOffset-int-int-) | Получает диапазон [Range](../../com.aspose.cells/range) со смещением. |
| [getRefersTo()](#getRefersTo--) | Получает то, на что ссылается диапазон. |
| [getRowCount()](#getRowCount--) | Получает количество строк в диапазоне. |
| [getRowHeight()](#getRowHeight--) | Устанавливает или получает высоту строк в этом диапазоне |
| [getTop()](#getTop--) | Получает расстояние в пунктах от верхнего края строки 1 до верхнего края диапазона. |
| [getValue()](#getValue--) | Получает значение диапазона. |
| [getWidth()](#getWidth--) | Получает ширину диапазона в пунктах. |
| [getWorksheet()](#getWorksheet--) | Получает объект [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--)object, который содержит этот диапазон. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range range)](#intersect-com.aspose.cells.Range-) | Возвращает объект [Range](../../com.aspose.cells/range), представляющий прямоугольное пересечение двух диапазонов. |
| [isBlank()](#isBlank--) | Указывает, содержит ли диапазон значения. |
| [isIntersect(Range range)](#isIntersect-com.aspose.cells.Range-) | Указывает, пересекается ли диапазон. |
| [iterator()](#iterator--) | Получает перечислитель ячеек в этом диапазоне. |
| [merge()](#merge--) | Объединяет диапазон ячеек в одну ячейку. |
| [moveTo(int destRow, int destColumn)](#moveTo-int-int-) | Перемещает текущий диапазон в целевой диапазон. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Помещает значение в диапазон; при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Устанавливает или получает ширину столбца этого диапазона |
| [setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)](#setInsideBorders-int-int-com.aspose.cells.CellsColor-) | Устанавливает внутренние границы диапазона. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя диапазона. |
| [setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)](#setOutlineBorder-int-int-com.aspose.cells.CellsColor-) | Устанавливает контурную границу вокруг диапазона ячеек. |
| [setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)](#setOutlineBorder-int-int-com.aspose.cells.Color-) | Устанавливает контурную границу вокруг диапазона ячеек. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | Устанавливает контурные границы вокруг диапазона ячеек с одинаковым стилем и цветом границы. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Устанавливает контурные границы вокруг диапазона ячеек с одинаковым стилем и цветом границы. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Устанавливает внешние границы вокруг диапазона ячеек. |
| [setRowHeight(double value)](#setRowHeight-double-) | Устанавливает или получает высоту строк в этом диапазоне |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Устанавливает стиль диапазона. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Применяет стиль ячейки. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Устанавливает значение диапазона. |
| [toHtml(HtmlSaveOptions saveOptions)](#toHtml-com.aspose.cells.HtmlSaveOptions-) | Преобразует диапазон в HTML. |
| [toImage(ImageOrPrintOptions options)](#toImage-com.aspose.cells.ImageOrPrintOptions-) | Преобразует диапазон в изображение. |
| [toJson(JsonSaveOptions options)](#toJson-com.aspose.cells.JsonSaveOptions-) | Преобразует диапазон в значение JSON. |
| [toString()](#toString--) | Возвращает строку, представляющую текущий объект Range. |
| [transpose()](#transpose--) | Транспонирует (поворачивает) данные из строк в столбцы и наоборот. |
| [unMerge()](#unMerge--) | Разъединяет объединённые ячейки этого диапазона. |
| [union(Range range)](#union-com.aspose.cells.Range-) | Возвращает объединение двух диапазонов. |
| [unionRang(Range range)](#unionRang-com.aspose.cells.Range-) | Возвращает результат объединения двух диапазонов. |
| [unionRanges(Range[] ranges)](#unionRanges-com.aspose.cells.Range---) | Возвращает результат объединения двух диапазонов. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Range(CellArea ca, Cells cells) {#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-}
```
public Range(CellArea ca, Cells cells)
```


Конструктор класса.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Диапазон. |
| cells | [Cells](../../com.aspose.cells/cells) |  |

### Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells) {#Range-int-int-int-int-com.aspose.cells.Cells-}
```
public Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)
```


Конструктор класса.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | int | Первая строка этого диапазона(нумерация с нуля) |
| firstColumn | int | Первая колонка этого диапазона (нумерация с нуля). |
| rowNumber | int | Количество строк(нумерация с 1) |
| columnNumber | int | Количество столбцов (нумерация с 1) |
| cells | [Cells](../../com.aspose.cells/cells) | Объект Range принадлежит этому объекту Cells. |

### addHyperlink(String address, String textToDisplay, String screenTip) {#addHyperlink-java.lang.String-java.lang.String-java.lang.String-}
```
public Hyperlink addHyperlink(String address, String textToDisplay, String screenTip)
```


Добавляет гиперссылку в указанную ячейку или диапазон ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| адрес | java.lang.String | Адрес гиперссылки. |
| textToDisplay | java.lang.String | Текст, который будет отображаться для указанной гиперссылки. |
| screenTip | java.lang.String | Текст подсказки (screenTip) для указанной гиперссылки. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - [Hyperlink](../../com.aspose.cells/hyperlink) object.
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Применяет форматы ко всему диапазону.

**Remarks**

Каждая ячейка в этом диапазоне будет содержать объект [Style](../../com.aspose.cells/style). Поэтому этот метод требует много памяти. Пожалуйста, используйте его осторожно.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Объект стиля, который будет применён. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Флаги, указывающие применённые свойства форматирования. |

### autoFill(Range target) {#autoFill-com.aspose.cells.Range-}
```
public void autoFill(Range target)
```


Автоматически заполняет целевой диапазон.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").putValue(1);
         cells.get("A2").putValue(2);
         Range source = cells.createRange("A1:A2");
         Range target = cells.createRange("A3:A10");
         //fill 3,4,5....10 to the range A3:A10
         source.autoFill(target);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | целевой диапазон. |

### autoFill(Range target, int autoFillType) {#autoFill-com.aspose.cells.Range-int-}
```
public void autoFill(Range target, int autoFillType)
```


Автоматически заполняет целевой диапазон.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | Целевой диапазон. |
| autoFillType | int | [AutoFillType](../../com.aspose.cells/autofilltype). Тип автозаполнения. |

### clear() {#clear--}
```
public void clear()
```


Очищает этот диапазон.

### clearComments() {#clearComments--}
```
public void clearComments()
```


Очищает комментарии этого диапазона.

### clearContents() {#clearContents--}
```
public void clearContents()
```


Очищает содержимое этого диапазона.

### clearFormats() {#clearFormats--}
```
public void clearFormats()
```


Очищает форматы этого диапазона.

### clearHyperlinks(boolean clearFormat) {#clearHyperlinks-boolean-}
```
public void clearHyperlinks(boolean clearFormat)
```


Только удаляет гиперссылки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| clearFormat | boolean | Указывает, следует ли очищать формат гиперссылок. |

### copy(Range range) {#copy-com.aspose.cells.Range-}
```
public void copy(Range range)
```


Копирует данные (включая формулы), форматирование, графические объекты и т.д. из исходного диапазона.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         Range range1 = cells.createRange("A1:A5");
         Range range2 = cells.createRange("A6:A10");
         //Copy the range.
         range1.copy(range2);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Объект исходного [Range](../../com.aspose.cells/range). |

### copy(Range range, PasteOptions options) {#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-}
```
public void copy(Range range, PasteOptions options)
```


Копирование диапазона с параметрами «Специальная вставка».

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Исходный диапазон. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | Параметры специальной вставки. |

### copyData(Range range) {#copyData-com.aspose.cells.Range-}
```
public void copyData(Range range)
```


Копирует данные ячеек (включая формулы) из исходного диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Объект исходного [Range](../../com.aspose.cells/range). |

### copyStyle(Range range) {#copyStyle-com.aspose.cells.Range-}
```
public void copyStyle(Range range)
```


Копирует настройки стиля из исходного диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Объект исходного [Range](../../com.aspose.cells/range). |

### copyValue(Range range) {#copyValue-com.aspose.cells.Range-}
```
public void copyValue(Range range)
```


Копирует значение ячейки из исходного диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Объект исходного [Range](../../com.aspose.cells/range). |

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
### get(int rowOffset, int columnOffset) {#get-int-int-}
```
public Cell get(int rowOffset, int columnOffset)
```


Получает объект [Cell](../../com.aspose.cells/cell) в этом диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | int | Смещение строки в этом диапазоне, начиная с нуля. |
| columnOffset | int | Смещение столбца в этом диапазоне, начиная с нуля. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getAddress() {#getAddress--}
```
public String getAddress()
```


Получает адрес диапазона.

**Returns:**
java.lang.String
### getCellOrNull(int rowOffset, int columnOffset) {#getCellOrNull-int-int-}
```
public Cell getCellOrNull(int rowOffset, int columnOffset)
```


Получает объект [Cell](../../com.aspose.cells/cell) или null в этом диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | int | Смещение строки в этом диапазоне, начиная с нуля. |
| columnOffset | int | Смещение столбца в этом диапазоне, начиная с нуля. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Получает количество столбцов в диапазоне.

**Returns:**
int
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


Устанавливает или получает ширину столбца этого диапазона

**Returns:**
double
### getCurrentRegion() {#getCurrentRegion--}
```
public Range getCurrentRegion()
```


Возвращает объект Range, представляющий текущий регион. Текущий регион — это диапазон, ограниченный любой комбинацией пустых строк и пустых столбцов.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireColumn() {#getEntireColumn--}
```
public Range getEntireColumn()
```


Получает объект Range, представляющий весь столбец (или столбцы), содержащий указанный диапазон.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireRow() {#getEntireRow--}
```
public Range getEntireRow()
```


Получает объект Range, представляющий всю строку (или строки), содержащую указанный диапазон.

**Returns:**
[Range](../../com.aspose.cells/range)
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


Получает индекс первого столбца диапазона.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


Получает индекс первой строки диапазона.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Получает ширину диапазона в пунктах.

**Returns:**
double
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


Получает все гиперссылки в диапазоне.

**Returns:**
com.aspose.cells.Hyperlink[]
### getLeft() {#getLeft--}
```
public double getLeft()
```


Получает расстояние в пунктах от левого края столбца A до левого края диапазона.

**Returns:**
double
### getName() {#getName--}
```
public String getName()
```


Получает имя диапазона.

**Remarks**

Поддерживается именованный диапазон. Например,

range.Name = "Sheet1!MyRange";

**Returns:**
java.lang.String
### getOffset(int rowOffset, int columnOffset) {#getOffset-int-int-}
```
public Range getOffset(int rowOffset, int columnOffset)
```


Получает диапазон [Range](../../com.aspose.cells/range) со смещением.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | int | Смещение строки в этом диапазоне, начиная с нуля. |
| columnOffset | int | Смещение столбца в этом диапазоне, начиная с нуля. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Получает то, на что ссылается диапазон.

**Returns:**
java.lang.String
### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Получает количество строк в диапазоне.

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


Устанавливает или получает высоту строк в этом диапазоне

**Returns:**
double
### getTop() {#getTop--}
```
public double getTop()
```


Получает расстояние в пунктах от верхнего края строки 1 до верхнего края диапазона.

**Returns:**
double
### getValue() {#getValue--}
```
public Object getValue()
```


Получает значение диапазона.

**Remarks**

Если диапазон содержит несколько ячеек, возвращаемый/применяемый объект должен быть Object[][].

**Returns:**
java.lang.Object
### getWidth() {#getWidth--}
```
public double getWidth()
```


Получает ширину диапазона в пунктах.

**Returns:**
double
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Получает объект [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--)object, который содержит этот диапазон.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range range) {#intersect-com.aspose.cells.Range-}
```
public Range intersect(Range range)
```


Возвращает объект [Range](../../com.aspose.cells/range), представляющий прямоугольное пересечение двух диапазонов.

**Remarks**

Если два диапазона не пересекаются, возвращает null.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         Range range1 = cells.createRange("A1:A5");
         Range range2 = cells.createRange("A3:A10");
         //Get intersected range of the two ranges.
         Range intersectRange = range1.intersect(range2);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Пересекающийся диапазон. |

**Returns:**
[Range](../../com.aspose.cells/range) - Returns a [Range](../../com.aspose.cells/range) object
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Указывает, содержит ли диапазон значения.

**Returns:**
boolean -
### isIntersect(Range range) {#isIntersect-com.aspose.cells.Range-}
```
public boolean isIntersect(Range range)
```


Указывает, пересекается ли диапазон.

**Remarks**

Если два диапазона находятся не в одном листе, возвращает false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Диапазон. |

**Returns:**
boolean - Является ли диапазон пересекающимся.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Получает перечислитель ячеек в этом диапазоне.

**Remarks**

При обходе элементов с помощью возвращённого Enumerator коллекцию ячеек не следует изменять(например, операции, которые создают новые Cell/Row или удаляют существующие Cell/Row). В противном случае enumerator может не суметь корректно пройти все ячейки(некоторые элементы могут быть пройдены несколько раз или пропущены).

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.createRange("B2:C3").iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - Enumerator ячеек
### merge() {#merge--}
```
public void merge()
```


Объединяет диапазон ячеек в одну ячейку.

**Remarks**

Ссылка на объединённую ячейку через адрес верхней‑левой ячейки в диапазоне.

### moveTo(int destRow, int destColumn) {#moveTo-int-int-}
```
public void moveTo(int destRow, int destColumn)
```


Перемещает текущий диапазон в целевой диапазон.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destRow | int | Начальная строка целевого диапазона. |
| destColumn | int | Начальный столбец целевого диапазона. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Помещает значение в диапазон; при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stringValue | java.lang.String | Входное значение |
| isConverted | boolean | True: преобразовано в другой тип данных, если это уместно. |
| setStyle | boolean | True: установить числовой формат в стиль ячейки при преобразовании в другой тип данных |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


Устанавливает или получает ширину столбца этого диапазона

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor) {#setInsideBorders-int-int-com.aspose.cells.CellsColor-}
```
public void setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)
```


Устанавливает внутренние границы диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Внутри типа границы могут быть только [BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) и [BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL). |
| lineStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Стиль границы. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Цвет границы. |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Устанавливает имя диапазона.

**Remarks**

Поддерживается именованный диапазон. Например,

range.Name = "Sheet1!MyRange";

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor) {#setOutlineBorder-int-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)
```


Устанавливает контурную границу вокруг диапазона ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Край границы. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Стиль границы. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Цвет границы. |

### setOutlineBorder(int borderEdge, int borderStyle, Color borderColor) {#setOutlineBorder-int-int-com.aspose.cells.Color-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)
```


Устанавливает контурную границу вокруг диапазона ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Край границы. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Стиль границы. |
| borderColor | [Color](../../com.aspose.cells/color) | Цвет границы. |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


Устанавливает контурные границы вокруг диапазона ячеек с одинаковым стилем и цветом границы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Стиль границы. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Цвет границы. |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Устанавливает контурные границы вокруг диапазона ячеек с одинаковым стилем и цветом границы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Стиль границы. |
| borderColor | [Color](../../com.aspose.cells/color) | Цвет границы. |

### setOutlineBorders(int[] borderStyles, Color[] borderColors) {#setOutlineBorders-int---com.aspose.cells.Color---}
```
public void setOutlineBorders(int[] borderStyles, Color[] borderColors)
```


Устанавливает внешние границы вокруг диапазона ячеек.

**Remarks**

Длина массива borderStyles должна быть 4. Порядок элементов borderStyles должен быть сверху, снизу, слева, справа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| borderStyles | int[] | [CellBorderType](../../com.aspose.cells/cellbordertype). Стили границы. |
| borderColors | [Color\[\]](../../com.aspose.cells/color) | Цвета границ. |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


Устанавливает или получает высоту строк в этом диапазоне

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Устанавливает стиль диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Объект Style. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


Применяет стиль ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Стиль ячейки. |
| explicitFlag | boolean | True, только перезаписывая форматирование, которое явно задано. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Устанавливает значение диапазона.

**Remarks**

Если диапазон содержит несколько ячеек, возвращаемый/применяемый объект должен быть Object[][].

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object |  |

### toHtml(HtmlSaveOptions saveOptions) {#toHtml-com.aspose.cells.HtmlSaveOptions-}
```
public byte[] toHtml(HtmlSaveOptions saveOptions)
```


Преобразует диапазон в HTML.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| saveOptions | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) | Параметры для преобразования диапазона в html. |

**Returns:**
byte[] -
### toImage(ImageOrPrintOptions options) {#toImage-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(ImageOrPrintOptions options)
```


Преобразует диапазон в изображение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Параметры для преобразования этого диапазона в изображение |

**Returns:**
byte[] -
### toJson(JsonSaveOptions options) {#toJson-com.aspose.cells.JsonSaveOptions-}
```
public String toJson(JsonSaveOptions options)
```


Преобразует диапазон в значение JSON.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | Параметры преобразования |

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


Возвращает строку, представляющую текущий объект Range.

**Returns:**
java.lang.String -
### transpose() {#transpose--}
```
public void transpose()
```


Транспонирует (поворачивает) данные из строк в столбцы и наоборот.

### unMerge() {#unMerge--}
```
public void unMerge()
```


Разъединяет объединённые ячейки этого диапазона.

### union(Range range) {#union-com.aspose.cells.Range-}
```
public ArrayList union(Range range)
```


Возвращает объединение двух диапазонов.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Range.UnionRanges(). Этот метод будет удалён через 12 месяцев, начиная с ноября 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Диапазон |

**Returns:**
java.util.ArrayList — объединение двух диапазонов.
### unionRang(Range range) {#unionRang-com.aspose.cells.Range-}
```
public Range[] unionRang(Range range)
```


Возвращает результат объединения двух диапазонов.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Range.UnionRanges(). Этот метод будет удалён через 12 месяцев, начиная с мая 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Диапазон |

**Returns:**
com.aspose.cells.Range[] — объединение двух диапазонов.
### unionRanges(Range[] ranges) {#unionRanges-com.aspose.cells.Range---}
```
public UnionRange unionRanges(Range[] ranges)
```


Возвращает результат объединения двух диапазонов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | Диапазон |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - The union of two ranges.
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

