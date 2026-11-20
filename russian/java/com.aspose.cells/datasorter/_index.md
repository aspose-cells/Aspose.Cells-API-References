---
title: "DataSorter"
second_title: "Справочник API Aspose.Cells for Java"
description: "Краткое описание для DataSorter."
type: docs
url: /ru/java/com.aspose.cells/datasorter/
---

**Inheritance:**
java.lang.Object
```
public class DataSorter
```

Краткое описание для DataSorter.

**Example**

```
         //Instantiate a new Workbook object.
         Workbook workbook = new Workbook("Book1.xls");
         //Get the workbook datasorter object.
         DataSorter sorter = workbook.getDataSorter();
         //Set the first order for datasorter object.
         sorter.setOrder1(com.aspose.cells.SortOrder.DESCENDING);
         //Define the first key.
         sorter.setKey1(0);
         //Set the second order for datasorter object.
         sorter.setOrder2(com.aspose.cells.SortOrder.ASCENDING);
         //Define the second key.
         sorter.setKey2(1);
         //Create a cells area (range).
         CellArea ca = new CellArea();
         //Specify the start row index.
         ca.StartRow = 0;
         //Specify the start column index.
         ca.StartColumn = 0;
         //Specify the last row index.
         ca.EndRow = 13;
         //Specify the last column index.
         ca.EndColumn = 1;
         //Sort data in the specified data range (A1:B14)
         sorter.sort(workbook.getWorksheets().get(0).getCells(), ca);
         //Save the excel file.
         workbook.save("outBook.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [addColorKey(int key, int type, int order, Color color)](#addColorKey-int-int-int-com.aspose.cells.Color-) | Добавляет цветовой ключ сортировки. |
| [addKey(int key, int order)](#addKey-int-int-) | Добавляет индекс отсортированного столбца и порядок сортировки. |
| [addKey(int key, int type, int order, Object customList)](#addKey-int-int-int-java.lang.Object-) | Добавляет индекс отсортированного столбца и порядок сортировки с пользовательским списком сортировки. |
| [addKey(int key, int order, String customList)](#addKey-int-int-java.lang.String-) | Добавляет индекс отсортированного столбца и порядок сортировки с пользовательским списком сортировки. |
| [addKey(int key, int order, String[] customList)](#addKey-int-int-java.lang.String---) | Добавляет индекс отсортированного столбца и порядок сортировки с пользовательским списком сортировки. |
| [clear()](#clear--) | Очистить все настройки. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Получает, чувствителен ли регистр при сравнении строк. |
| [getClass()](#getClass--) |  |
| [getKey1()](#getKey1--) | Представляет индекс первого отсортированного столбца (абсолютная позиция, столбец A = 0, B = 1, ...) |
| [getKey2()](#getKey2--) | Представляет индекс второго отсортированного столбца (абсолютная позиция, столбец A = 0, B = 1, ...) |
| [getKey3()](#getKey3--) | Представляет индекс третьего отсортированного столбца (абсолютная позиция, столбец A = 0, B = 1, ...) |
| [getKeys()](#getKeys--) | Получает список ключей сортировщика данных. |
| [getOrder1()](#getOrder1--) | Представляет порядок сортировки первого ключа. |
| [getOrder2()](#getOrder2--) | Представляет порядок сортировки второго ключа. |
| [getOrder3()](#getOrder3--) | Представляет порядок сортировки третьего ключа. |
| [getSortAsNumber()](#getSortAsNumber--) | Указывает, следует ли сортировать всё, что выглядит как число. |
| [getSortLeftToRight()](#getSortLeftToRight--) | True означает, что ориентация сортировки слева направо. |
| [hasHeaders()](#hasHeaders--) | Представляет, имеет ли диапазон заголовки. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Устанавливает, чувствителен ли регистр при сравнении строк. |
| [setHasHeaders(boolean value)](#setHasHeaders-boolean-) | Представляет, имеет ли диапазон заголовки. |
| [setKey1(int value)](#setKey1-int-) | Представляет индекс первого отсортированного столбца (абсолютная позиция, столбец A = 0, B = 1, ...) |
| [setKey2(int value)](#setKey2-int-) | Представляет индекс второго отсортированного столбца (абсолютная позиция, столбец A = 0, B = 1, ...) |
| [setKey3(int value)](#setKey3-int-) | Представляет индекс третьего отсортированного столбца (абсолютная позиция, столбец A = 0, B = 1, ...) |
| [setOrder1(int value)](#setOrder1-int-) | Представляет порядок сортировки первого ключа. |
| [setOrder2(int value)](#setOrder2-int-) | Представляет порядок сортировки второго ключа. |
| [setOrder3(int value)](#setOrder3-int-) | Представляет порядок сортировки третьего ключа. |
| [setSortAsNumber(boolean value)](#setSortAsNumber-boolean-) | Указывает, следует ли сортировать всё, что выглядит как число. |
| [setSortLeftToRight(boolean value)](#setSortLeftToRight-boolean-) | True означает, что ориентация сортировки слева направо. |
| [sort()](#sort--) | Сортировать данные в диапазоне. |
| [sort(Cells cells, CellArea area)](#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-) | Отсортировать данные области. |
| [sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)](#sort-com.aspose.cells.Cells-int-int-int-int-) | Сортирует данные области. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColorKey(int key, int type, int order, Color color) {#addColorKey-int-int-int-com.aspose.cells.Color-}
```
public void addColorKey(int key, int type, int order, Color color)
```


Добавляет цветовой ключ сортировки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ключ | int | Индекс отсортированного столбца(абсолютная позиция, столбец A = 0, B = 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). Тип отсортированного значения цвета. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Порядок сортировки. |
| color | [Color](../../com.aspose.cells/color) | Пользовательский цвет сортировки. |

### addKey(int key, int order) {#addKey-int-int-}
```
public void addKey(int key, int order)
```


Добавляет индекс отсортированного столбца и порядок сортировки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ключ | int | Индекс отсортированного столбца(абсолютная позиция, столбец A = 0, B = 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Порядок сортировки |

### addKey(int key, int type, int order, Object customList) {#addKey-int-int-int-java.lang.Object-}
```
public void addKey(int key, int type, int order, Object customList)
```


Добавляет индекс отсортированного столбца и порядок сортировки с пользовательским списком сортировки.

**Remarks**

Если тип равен SortOnType.CellColor или SortOnType.FontColor, customList имеет тип Color.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ключ | int | Индекс отсортированного столбца(абсолютная позиция, столбец A = 0, B = 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). Тип отсортированного значения. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Порядок сортировки. |
| customList | java.lang.Object | Пользовательский список сортировки. |

### addKey(int key, int order, String customList) {#addKey-int-int-java.lang.String-}
```
public void addKey(int key, int order, String customList)
```


Добавляет индекс отсортированного столбца и порядок сортировки с пользовательским списком сортировки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ключ | int | Индекс отсортированного столбца(абсолютная позиция, столбец A = 0, B = 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Порядок сортировки. |
| customList | java.lang.String | Пользовательский список сортировки. |

### addKey(int key, int order, String[] customList) {#addKey-int-int-java.lang.String---}
```
public void addKey(int key, int order, String[] customList)
```


Добавляет индекс отсортированного столбца и порядок сортировки с пользовательским списком сортировки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ключ | int | Индекс отсортированного столбца(абсолютная позиция, столбец A = 0, B = 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Порядок сортировки. |
| customList | java.lang.String[] | Пользовательский список сортировки. |

### clear() {#clear--}
```
public void clear()
```


Очистить все настройки.

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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


Получает, чувствителен ли регистр при сравнении строк.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getKey1() {#getKey1--}
```
public int getKey1()
```


Представляет индекс первого отсортированного столбца (абсолютная позиция, столбец A = 0, B = 1, ...)

**Returns:**
int
### getKey2() {#getKey2--}
```
public int getKey2()
```


Представляет индекс второго отсортированного столбца (абсолютная позиция, столбец A = 0, B = 1, ...)

**Returns:**
int
### getKey3() {#getKey3--}
```
public int getKey3()
```


Представляет индекс третьего отсортированного столбца (абсолютная позиция, столбец A = 0, B = 1, ...)

**Returns:**
int
### getKeys() {#getKeys--}
```
public DataSorterKeyCollection getKeys()
```


Получает список ключей сортировщика данных.

**Returns:**
[DataSorterKeyCollection](../../com.aspose.cells/datasorterkeycollection)
### getOrder1() {#getOrder1--}
```
public int getOrder1()
```


Представляет порядок сортировки первого ключа.

См. [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getOrder2() {#getOrder2--}
```
public int getOrder2()
```


Представляет порядок сортировки второго ключа.

См. [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getOrder3() {#getOrder3--}
```
public int getOrder3()
```


Представляет порядок сортировки третьего ключа.

См. [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getSortAsNumber() {#getSortAsNumber--}
```
public boolean getSortAsNumber()
```


Указывает, следует ли сортировать всё, что выглядит как число.

**Returns:**
boolean
### getSortLeftToRight() {#getSortLeftToRight--}
```
public boolean getSortLeftToRight()
```


True означает, что ориентация сортировки слева направо. False означает, что ориентация сортировки сверху вниз. Значение по умолчанию — false.

**Returns:**
boolean
### hasHeaders() {#hasHeaders--}
```
public boolean hasHeaders()
```


Представляет, имеет ли диапазон заголовки.

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




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


Устанавливает, чувствителен ли регистр при сравнении строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasHeaders(boolean value) {#setHasHeaders-boolean-}
```
public void setHasHeaders(boolean value)
```


Представляет, имеет ли диапазон заголовки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setKey1(int value) {#setKey1-int-}
```
public void setKey1(int value)
```


Представляет индекс первого отсортированного столбца (абсолютная позиция, столбец A = 0, B = 1, ...)

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setKey2(int value) {#setKey2-int-}
```
public void setKey2(int value)
```


Представляет индекс второго отсортированного столбца (абсолютная позиция, столбец A = 0, B = 1, ...)

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setKey3(int value) {#setKey3-int-}
```
public void setKey3(int value)
```


Представляет индекс третьего отсортированного столбца (абсолютная позиция, столбец A = 0, B = 1, ...)

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setOrder1(int value) {#setOrder1-int-}
```
public void setOrder1(int value)
```


Представляет порядок сортировки первого ключа.

См. [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setOrder2(int value) {#setOrder2-int-}
```
public void setOrder2(int value)
```


Представляет порядок сортировки второго ключа.

См. [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setOrder3(int value) {#setOrder3-int-}
```
public void setOrder3(int value)
```


Представляет порядок сортировки третьего ключа.

См. [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSortAsNumber(boolean value) {#setSortAsNumber-boolean-}
```
public void setSortAsNumber(boolean value)
```


Указывает, следует ли сортировать всё, что выглядит как число.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSortLeftToRight(boolean value) {#setSortLeftToRight-boolean-}
```
public void setSortLeftToRight(boolean value)
```


True означает, что ориентация сортировки слева направо. False означает, что ориентация сортировки сверху вниз. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### sort() {#sort--}
```
public int[] sort()
```


Сортировать данные в диапазоне.

**Returns:**
int[] - оригинальные индексы(абсолютная позиция, например, столбец A = 0, B = 1, ...) отсортированных строк/столбцов. Если ни одна строка/столбец не требуется перемещать этой операцией сортировки, будет возвращено null.
### sort(Cells cells, CellArea area) {#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-}
```
public int[] sort(Cells cells, CellArea area)
```


Отсортировать данные области.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | Ячейки содержат область данных. |
| area | [CellArea](../../com.aspose.cells/cellarea) | Область, необходимая для сортировки |

**Returns:**
int[] - оригинальные индексы(абсолютная позиция, например, столбец A = 0, B = 1, ...) отсортированных строк/столбцов. Если ни одна строка/столбец не требуется перемещать этой операцией сортировки, будет возвращено null.
### sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn) {#sort-com.aspose.cells.Cells-int-int-int-int-}
```
public int[] sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```


Сортирует данные области.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | Ячейки содержат область данных. |
| startRow | int | Начальная строка области. |
| startColumn | int | Начальный столбец области. |
| endRow | int | Конечная строка области. |
| endColumn | int | Конечный столбец области. |

**Returns:**
int[] - оригинальные индексы(абсолютная позиция, например, столбец A = 0, B = 1, ...) отсортированных строк/столбцов. Если ни одна строка/столбец не требуется перемещать этой операцией сортировки, будет возвращено null.
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

