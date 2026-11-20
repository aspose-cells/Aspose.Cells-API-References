---
title: "CellArea"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет область ячеек."
type: docs
url: /ru/java/com.aspose.cells/cellarea/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public final class CellArea implements Comparable
```

Представляет область ячеек.

**Example**

```
         //Create Cell Area
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [CellArea()](#CellArea--) |  |
## Поля

| Поле | Описание |
| --- | --- |
| [EndColumn](#EndColumn) | Получает или задает конечный столбец этой области. |
| [EndRow](#EndRow) | Получает или задает конечную строку этой области. |
| [StartColumn](#StartColumn) | Получает или задает начальный столбец этой области. |
| [StartRow](#StartRow) | Получает или задает начальную строку этой области. |
## Методы

| Метод | Описание |
| --- | --- |
| [compareTo(Object obj)](#compareTo-java.lang.Object-) | Сравнивает два объекта CellArea по их верхнему левому углу. |
| [createCellArea(int startRow, int startColumn, int endRow, int endColumn)](#createCellArea-int-int-int-int-) | Создаёт область ячеек. |
| [createCellArea(String startCellName, String endCellName)](#createCellArea-java.lang.String-java.lang.String-) | Создаёт область ячеек. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Возвращает строку, представляющую текущий объект области ячеек. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellArea() {#CellArea--}
```
public CellArea()
```


### EndColumn {#EndColumn}
```
public int EndColumn
```


Получает или задает конечный столбец этой области.

### EndRow {#EndRow}
```
public int EndRow
```


Получает или задает конечную строку этой области.

### StartColumn {#StartColumn}
```
public int StartColumn
```


Получает или задает начальный столбец этой области.

### StartRow {#StartRow}
```
public int StartRow
```


Получает или задает начальную строку этой области.

### compareTo(Object obj) {#compareTo-java.lang.Object-}
```
public int compareTo(Object obj)
```


Сравнивает два объекта CellArea по их верхнему левому углу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
int — Если два угла находятся в разных строках, сравнивается их индекс строки. В противном случае сравнивается их индекс столбца. Если два угла одинаковы, возвращается 0.
### createCellArea(int startRow, int startColumn, int endRow, int endColumn) {#createCellArea-int-int-int-int-}
```
public static CellArea createCellArea(int startRow, int startColumn, int endRow, int endColumn)
```


Создаёт область ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Начальная строка. |
| startColumn | int | Начальный столбец. |
| endRow | int | Конечная строка. |
| endColumn | int | Конечный столбец. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
### createCellArea(String startCellName, String endCellName) {#createCellArea-java.lang.String-java.lang.String-}
```
public static CellArea createCellArea(String startCellName, String endCellName)
```


Создаёт область ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startCellName | java.lang.String | Верхняя‑левая ячейка диапазона. |
| endCellName | java.lang.String | Ячейка диапазона в правом нижнем углу. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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




### toString() {#toString--}
```
public String toString()
```


Возвращает строку, представляющую текущий объект области ячеек.

**Returns:**
java.lang.String -
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

