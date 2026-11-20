---
title: "Row"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет одну строку в листе."
type: docs
url: /ru/java/com.aspose.cells/row/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Row implements Iterable
```

Представляет одну строку в листе.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setBackgroundColor(Color.getBlue());
 
         //Setting the foreground color to Red
         style.setForegroundColor(Color.getRed());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.DIAGONAL_STRIPE);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
          //Apply Style to first row
         row.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Применяет форматирование ко всей строке. |
| [copySettings(Row source, boolean checkStyle)](#copySettings-com.aspose.cells.Row-boolean-) | Копировать настройки строки, такие как стиль, высота, видимость и т.д. |
| [equals(Row row)](#equals-com.aspose.cells.Row-) | Проверяет, ссылается ли этот объект на ту же строку, что и другой объект строки. |
| [equals(Object obj)](#equals-java.lang.Object-) | Проверяет, ссылается ли этот объект на ту же строку, что и другой. |
| [get(int column)](#get-int-) | Получает ячейку. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Получить ячейку по определённому индексу в коллекции ячеек этой строки. |
| [getCellOrNull(int column)](#getCellOrNull-int-) | Получает ячейку или null по указанному индексу. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Получает первый объект ячейки в строке. |
| [getFirstDataCell()](#getFirstDataCell--) | Получает первую непустую ячейку в строке. |
| [getGroupLevel()](#getGroupLevel--) | Получает уровень группы строки. |
| [getHeight()](#getHeight--) | Получает высоту строки в единицах Points. |
| [getIndex()](#getIndex--) | Получает индекс этой строки. |
| [getLastCell()](#getLastCell--) | Получает последний объект ячейки в строке. |
| [getLastDataCell()](#getLastDataCell--) | Получает последнюю непустую ячейку в строке. |
| [getStyle()](#getStyle--) | Получает стиль этой строки. |
| [hasCustomStyle()](#hasCustomStyle--) | Указывает, имеет ли эта строка пользовательские настройки стиля (отличные от стандартных, унаследованных из книги). |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Указывает, содержит ли строка какие-либо данные |
| [isCollapsed()](#isCollapsed--) | свёрнута ли строка |
| [isHeightMatched()](#isHeightMatched--) | Указывает, соответствует ли высота строки текущим настройкам шрифта по умолчанию в книге. |
| [isHidden()](#isHidden--) | Указывает, скрыта ли строка. |
| [iterator()](#iterator--) | Получает перечислитель ячеек |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Получает перечислитель, который перебирает ячейки в этой строке. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | свёрнута ли строка |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Получает уровень группы строки. |
| [setHeight(double value)](#setHeight-double-) | Устанавливает высоту строки в единицах точек. |
| [setHeightMatched(boolean value)](#setHeightMatched-boolean-) | Указывает, соответствует ли высота строки текущим настройкам шрифта по умолчанию в книге. |
| [setHidden(boolean value)](#setHidden-boolean-) | Указывает, скрыта ли строка. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Устанавливает стиль этой строки. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Применяет форматирование ко всей строке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Объект стиля, который будет применён. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Флаги, указывающие применённые свойства форматирования. |

### copySettings(Row source, boolean checkStyle) {#copySettings-com.aspose.cells.Row-boolean-}
```
public void copySettings(Row source, boolean checkStyle)
```


Копировать настройки строки, такие как стиль, высота, видимость и т.д.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | [Row](../../com.aspose.cells/row) | исходная строка, настройки которой будут скопированы в эту |
| checkStyle | boolean | проверять и собирать стиль. Действует и требуется только когда два объекта строки принадлежат разным книгам и стили этих книг различаются. |

### equals(Row row) {#equals-com.aspose.cells.Row-}
```
public boolean equals(Row row)
```


Проверяет, ссылается ли этот объект на ту же строку, что и другой объект строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | другой объект строки |

**Returns:**
логический - true, если два объекта строки ссылаются на одну и ту же строку.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Проверяет, ссылается ли этот объект на ту же строку, что и другой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object | другой объект |

**Returns:**
логический - true, если два объекта ссылаются на одну и ту же строку.
### get(int column) {#get-int-}
```
public Cell get(int column)
```


Получает ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца |

**Returns:**
[Cell](../../com.aspose.cells/cell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public Cell getCellByIndex(int index)
```


Получить ячейку по определённому индексу в коллекции ячеек этой строки.

**Remarks**

Для последовательного обхода всех ячеек без изменения использование [iterator()](../../com.aspose.cells/row\#iterator--) обеспечит лучшую производительность, чем получение ячеек по одной этим методом.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс (позиция) ячейки в коллекции ячеек этой строки. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The Cell object at given position.
### getCellOrNull(int column) {#getCellOrNull-int-}
```
public Cell getCellOrNull(int column)
```


Получает ячейку или null по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Returns the cell object if the cell exists. Or returns null if the cell object does not exist.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Получает первый объект ячейки в строке.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataCell() {#getFirstDataCell--}
```
public Cell getFirstDataCell()
```


Получает первую непустую ячейку в строке.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Получает уровень группы строки.

**Returns:**
byte
### getHeight() {#getHeight--}
```
public double getHeight()
```


Получает высоту строки в единицах Points.

**Returns:**
double
### getIndex() {#getIndex--}
```
public int getIndex()
```


Получает индекс этой строки.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Получает последний объект ячейки в строке.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataCell() {#getLastDataCell--}
```
public Cell getLastDataCell()
```


Получает последнюю непустую ячейку в строке.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Получает стиль этой строки.

**Remarks**

Изменение возвращённого объекта стиля напрямую не оказывает влияния на эту строку или её ячейки. Необходимо вызвать метод [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-) или [setStyle(Style)](../../com.aspose.cells/row\#setStyle-Style-) для применения изменений к этой строке.

Стиль строки — это стиль, который будет наследоваться ячейками в этой строке (те ячейки, у которых нет пользовательских настроек стиля, такие как существующие ячейки, для которых стиль не был явно установлен, или ячейки, которые ещё не созданы).

**Returns:**
[Style](../../com.aspose.cells/style)
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Указывает, имеет ли эта строка пользовательские настройки стиля (отличные от стандартных, унаследованных из книги).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Указывает, содержит ли строка какие-либо данные

**Returns:**
boolean
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


свёрнута ли строка

**Returns:**
boolean
### isHeightMatched() {#isHeightMatched--}
```
public boolean isHeightMatched()
```


Указывает, соответствует ли высота строки текущим настройкам шрифта по умолчанию в книге. Значение true этого свойства также означает, что высота строки "автоматическая" без пользовательского значения высоты.

**Remarks**

Когда это свойство истинно, при изменении содержимого строки обычно требуется пересчитать высоту строки (например, с помощью [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)), чтобы получить тот же результат, что отображается в MS Excel при открытии книги.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Указывает, скрыта ли строка.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Получает перечислитель ячеек

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().get(1).iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - Перечислитель ячеек, который будет обходить все существующие ячейки в этой строке.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


Получает перечислитель, который перебирает ячейки в этой строке.

**Remarks**

Если строка будет изменена (операциями, которые могут привести к созданию новой ячейки или удалению существующей) во время обхода с помощью перечислителя, следует использовать синхронизированный перечислитель вместо обычного, чтобы обход мог продолжаться с позиции сразу после последней пройденной методом MoveNext(). При этом, помимо преимущества, что ни один элемент не будет пропущен или пройден несколько раз, недостатком синхронизированного перечислителя является небольшое снижение производительности по сравнению с обычным.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| обратный | boolean | нужно ли перечислять ячейки в обратном порядке |
| синхронный | boolean | нужно ли возвращаемому перечислителю проверять изменения ячеек в этой строке и поддерживать синхронизацию с ними. |

**Returns:**
java.util.Iterator - Перечислитель ячеек, который будет обходить все существующие ячейки в этой строке.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


свёрнута ли строка

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


Получает уровень группы строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Устанавливает высоту строки в единицах точек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setHeightMatched(boolean value) {#setHeightMatched-boolean-}
```
public void setHeightMatched(boolean value)
```


Указывает, соответствует ли высота строки текущим настройкам шрифта по умолчанию в книге. Значение true этого свойства также означает, что высота строки "автоматическая" без пользовательского значения высоты.

**Remarks**

Когда это свойство истинно, при изменении содержимого строки обычно требуется пересчитать высоту строки (например, с помощью [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)), чтобы получить тот же результат, что отображается в MS Excel при открытии книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Указывает, скрыта ли строка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Устанавливает стиль этой строки.

**Remarks**

Этот метод только задает указанный стиль как стиль по умолчанию для этой строки, не изменяя настройки стиля для существующих ячеек в этой строке. Чтобы одновременно обновить настройки стиля существующих ячеек до указанного стиля, пожалуйста, используйте [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-)

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | стиль, который будет использоваться как стиль по умолчанию для ячеек в этой строке. |

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

