---
title: "CalculationCell"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет данные, связанные с вычислением одной ячейки, которая вычисляется."
type: docs
url: /ru/java/com.aspose.cells/calculationcell/
---

**Inheritance:**
java.lang.Object
```
public class CalculationCell
```

Представляет данные, связанные с вычислением одной ячейки, которая вычисляется.

**Remarks**

Пользователь не должен изменять какие-либо данные в Workbook во время процесса вычисления формул, иначе могут возникнуть неожиданные результаты или исключения. Поэтому все объекты, предоставляемые этим классом (например, объект Cell метода [getCell()](../../com.aspose.cells/calculationcell\\#getCell--)) предназначены только для \"read\".
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Получает объект Cell, который вычисляется. |
| [getCellColumn()](#getCellColumn--) | Получает индекс столбца ячейки. |
| [getCellRow()](#getCellRow--) | Получает индекс строки ячейки. |
| [getClass()](#getClass--) |  |
| [getWorkbook()](#getWorkbook--) | Получает объект Workbook. |
| [getWorksheet()](#getWorksheet--) | Получает объект Worksheet, в котором находится ячейка. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object v)](#setCalculatedValue-java.lang.Object-) | Устанавливает вычисленное значение для ячейки. |
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
### getCell() {#getCell--}
```
public Cell getCell()
```


Получает объект Cell, который вычисляется.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


Получает индекс столбца ячейки.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


Получает индекс строки ячейки.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Получает объект Workbook.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Получает объект Worksheet, в котором находится ячейка.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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




### setCalculatedValue(Object v) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object v)
```


Устанавливает вычисленное значение для ячейки.

**Remarks**

Пользователь может установить вычисленный результат с помощью этого метода, чтобы игнорировать автоматический расчет для ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| v | java.lang.Object |  |

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

