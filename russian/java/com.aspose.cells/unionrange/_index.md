---
title: "UnionRange"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет объединённый диапазон."
type: docs
url: /ru/java/com.aspose.cells/unionrange/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class UnionRange implements Iterable
```

Представляет объединённый диапазон.
## Методы

| Метод | Описание |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Применяет форматы ко всему диапазону. |
| [copy(UnionRange range, PasteOptions options)](#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-) | Копирование диапазона с параметрами «Специальная вставка». |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellCount()](#getCellCount--) | Получает общее количество ячеек в диапазоне. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Получает количество строк в диапазоне. |
| [getFirstColumn()](#getFirstColumn--) | Получает индекс первого столбца диапазона. |
| [getFirstRow()](#getFirstRow--) | Получает индекс первой строки диапазона. |
| [getHyperlinks()](#getHyperlinks--) | Получает все гиперссылки в диапазоне. |
| [getName()](#getName--) | Получает имя диапазона. |
| [getRangeCount()](#getRangeCount--) | Получает количество диапазонов. |
| [getRanges()](#getRanges--) | Получает все объединённые диапазоны. |
| [getRefersTo()](#getRefersTo--) | Получает то, на что ссылается диапазон. |
| [getRowCount()](#getRowCount--) | Получает количество строк в диапазоне. |
| [getValue()](#getValue--) | Получает значения диапазона. |
| [hasRange()](#hasRange--) | Указывает, имеет ли это диапазон. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range[] ranges)](#intersect-com.aspose.cells.Range---) | Пересекает другой диапазон. |
| [intersect(UnionRange unionRange)](#intersect-com.aspose.cells.UnionRange-) | Пересекает другой диапазон. |
| [intersect(String range)](#intersect-java.lang.String-) | Пересекает другой диапазон. |
| [iterator()](#iterator--) | Получает перечислитель ячеек в этом диапазоне. |
| [merge()](#merge--) | Объединяет диапазон ячеек в одну ячейку. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Помещает значение в диапазон; при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя диапазона. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Устанавливает контурные границы вокруг диапазона ячеек с одинаковым стилем и цветом границы. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Устанавливает внешние границы вокруг диапазона ячеек. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Устанавливает стиль диапазона. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Устанавливает значения диапазона. |
| [toString()](#toString--) |  |
| [unMerge()](#unMerge--) | Разъединяет объединённые ячейки этого диапазона. |
| [union(Range[] ranges)](#union-com.aspose.cells.Range---) | Объединить диапазоны. |
| [union(UnionRange unionRange)](#union-com.aspose.cells.UnionRange-) | Объединить другой диапазон. |
| [union(String range)](#union-java.lang.String-) | Объединить другой диапазон. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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

### copy(UnionRange range, PasteOptions options) {#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-}
```
public void copy(UnionRange range, PasteOptions options)
```


Копирование диапазона с параметрами «Специальная вставка».

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [UnionRange](../../com.aspose.cells/unionrange) | Исходный диапазон. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | Параметры специальной вставки. |

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
### getCellCount() {#getCellCount--}
```
public int getCellCount()
```


Получает общее количество ячеек в диапазоне.

**Returns:**
int
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


Получает количество строк в диапазоне.

**Remarks**

Действует только когда содержит один диапазон.

**Returns:**
int
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


Получает индекс первого столбца диапазона.

**Remarks**

Действует только когда содержит один диапазон.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


Получает индекс первой строки диапазона.

**Remarks**

Действует только когда содержит один диапазон.

**Returns:**
int
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


Получает все гиперссылки в диапазоне.

**Returns:**
com.aspose.cells.Hyperlink[]
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
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


Получает количество диапазонов.

**Returns:**
int
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


Получает все объединённые диапазоны.

**Returns:**
com.aspose.cells.Range[]
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

**Remarks**

Действует только когда содержит один диапазон.

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Получает значения диапазона.

**Returns:**
java.lang.Object
### hasRange() {#hasRange--}
```
public boolean hasRange()
```


Указывает, имеет ли это диапазон.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range[] ranges) {#intersect-com.aspose.cells.Range---}
```
public UnionRange intersect(Range[] ranges)
```


Пересекает другой диапазон.

**Remarks**

Если два объединённых диапазона не пересекаются, возвращает null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | Диапазон. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(UnionRange unionRange) {#intersect-com.aspose.cells.UnionRange-}
```
public UnionRange intersect(UnionRange unionRange)
```


Пересекает другой диапазон.

**Remarks**

Если два объединённых диапазона не пересекаются, возвращает null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | Диапазон. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(String range) {#intersect-java.lang.String-}
```
public UnionRange intersect(String range)
```


Пересекает другой диапазон.

**Remarks**

Если два объединённых диапазона не пересекаются, возвращает null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазон | java.lang.String | Диапазон. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### iterator() {#iterator--}
```
public Iterator iterator()
```


Получает перечислитель ячеек в этом диапазоне.

**Remarks**

При обходе элементов с помощью возвращённого Enumerator коллекцию ячеек не следует изменять(например, операции, которые создают новые Cell/Row или удаляют существующие Cell/Row). В противном случае enumerator может не суметь корректно пройти все ячейки(некоторые элементы могут быть пройдены несколько раз или пропущены).

**Returns:**
java.util.Iterator - Enumerator ячеек
### merge() {#merge--}
```
public void merge()
```


Объединяет диапазон ячеек в одну ячейку.

**Remarks**

Ссылка на объединённую ячейку через адрес верхней‑левой ячейки в диапазоне.

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

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Устанавливает стиль диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Объект Style. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Устанавливает значения диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unMerge() {#unMerge--}
```
public void unMerge()
```


Разъединяет объединённые ячейки этого диапазона.

### union(Range[] ranges) {#union-com.aspose.cells.Range---}
```
public UnionRange union(Range[] ranges)
```


Объединить диапазоны.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | Диапазоны. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(UnionRange unionRange) {#union-com.aspose.cells.UnionRange-}
```
public UnionRange union(UnionRange unionRange)
```


Объединить другой диапазон.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | Диапазон. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(String range) {#union-java.lang.String-}
```
public UnionRange union(String range)
```


Объединить другой диапазон.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазон | java.lang.String | Диапазон. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
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

