---
title: "CalculationData"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет необходимые данные при вычислении функции, таких как имя функции, параметры … и т.д."
type: docs
url: /ru/java/com.aspose.cells/calculationdata/
---

**Inheritance:**
java.lang.Object
```
public class CalculationData
```

Представляет необходимые данные при вычислении функции, такие как имя функции, параметры и т.д.

**Remarks**

Все объекты, предоставляемые этим классом, предназначены только для "read". Пользователь не должен изменять какие-либо данные в Workbook во время процесса вычисления формул, иначе могут возникнуть неожиданные результаты или Exception.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Получает вычисленное значение этой функции. |
| [getCell()](#getCell--) | Получает объект Cell, в котором находится функция. |
| [getCellColumn()](#getCellColumn--) | Получает индекс столбца ячейки, в которой находится функция. |
| [getCellRow()](#getCellRow--) | Получает индекс строки ячейки, в которой находится функция. |
| [getClass()](#getClass--) |  |
| [getFunctionName()](#getFunctionName--) | Получает имя функции, которую нужно вычислить. |
| [getParamCount()](#getParamCount--) | Получает количество параметров |
| [getParamText(int index)](#getParamText-int-) | Получает буквальный текст параметра по заданному индексу. |
| [getParamValue(int index)](#getParamValue-int-) | Получает представленный объект значения параметра по заданному индексу. |
| [getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)](#getParamValueInArrayMode-int-int-int-) | Получает значение(я) параметра по заданному индексу. |
| [getWorkbook()](#getWorkbook--) | Получает объект Workbook, в котором находится функция. |
| [getWorksheet()](#getWorksheet--) | Получает объект Worksheet, в котором находится функция. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object value)](#setCalculatedValue-java.lang.Object-) | Устанавливает вычисленное значение для этой функции. |
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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


Получает вычисленное значение этой функции.

**Remarks**

Пользователь должен установить это свойство в своем пользовательском движке вычислений для тех функций, которые поддерживает движок, и установленное значение будет возвращено при последующем получении этого свойства. Установленное значение может быть одним из возможных типов: [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), массивом таких значений, или объектом Range, Name, ReferredArea. Получение этого свойства до установки значения приведет к вычислению функции движком вычислений по умолчанию Aspose.Cells, после чего будет возвращено вычисленное значение (обычно это будет \#NAME? для пользовательских функций).

**Returns:**
java.lang.Object
### getCell() {#getCell--}
```
public Cell getCell()
```


Получает объект Cell, в котором находится функция.

**Remarks**

При вычислении формулы без установки её в ячейку, например с помощью [Worksheet.calculateFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateFormula-String-CalculationOptions-), формула будет вычислена так, как если бы она была записана в ячейку A1, поэтому оба метода [getCellRow()](../../com.aspose.cells/calculationdata\#getCellRow--) и [getCellColumn()](../../com.aspose.cells/calculationdata\#getCellColumn--) возвращают 0. Однако ячейка A1 на листе может не быть создана. Поэтому в такой ситуации это свойство будет иметь значение null.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


Получает индекс столбца ячейки, в которой находится функция.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


Получает индекс строки ячейки, в которой находится функция.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFunctionName() {#getFunctionName--}
```
public String getFunctionName()
```


Получает имя функции, которую нужно вычислить.

**Returns:**
java.lang.String
### getParamCount() {#getParamCount--}
```
public int getParamCount()
```


Получает количество параметров

**Returns:**
int
### getParamText(int index) {#getParamText-int-}
```
public String getParamText(int index)
```


Получает буквальный текст параметра по заданному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | индекс параметра (нумерация с нуля) |

**Returns:**
java.lang.String — буквальный текст параметра.
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


Получает представленный объект значения параметра по заданному индексу.

**Remarks**

Для одного параметра:

Если это простое значение, то возвращается само простое значение;

Если это ссылка, то возвращается объект ReferredArea;

Если она ссылается на набор(ы) данных с несколькими значениями, то возвращается массив объектов;

Если это некоторый вид выражения, требующего вычисления, то оно будет вычислено в режиме значения, и обычно будет возвращено одно значение в соответствии с текущей ячейкой. Например, если один параметр формулы D2 — это A:A+B:B, то будет вычислено и возвращено A2+B2. Однако если этот параметр указан в режиме массива (через  или ), то будет возвращён массив (object[][]), элементы которого — A1+B1, A2+B2, ….

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс параметра (нумерация с нуля) |

**Returns:**
java.lang.Object — вычисленное значение параметра.
### getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount) {#getParamValueInArrayMode-int-int-int-}
```
public Object[][] getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```


Получает значение(я) параметра по заданному индексу. Если параметр представляет собой выражение, требующее вычисления, то оно будет вычислено в режиме массива.

**Remarks**

Для выражения, которое необходимо вычислить, возьмём в качестве примера A:A+B:B: в режиме значения оно будет вычислено в одно значение в соответствии с текущей ячейкой. Но в режиме массива будут вычислены все значения A1+B1, A2+B2, A3+B3, … и использованы для построения возвращаемого массива. И в такой ситуации рекомендуется задать ограничения на количество строк/столбцов (например, согласно [Cells.getMaxDataRow()](../../com.aspose.cells/cells\#getMaxDataRow--) и [Cells.getMaxDataColumn()](../../com.aspose.cells/cells\#getMaxDataColumn--)), иначе возвращаемый большой массив может увеличить расход памяти из‑за большого количества бесполезных данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс параметра (нумерация с нуля) |
| maxRowCount | int | Ограничение количества строк в возвращаемом массиве. Если оно неположительное или превышает фактическое количество строк, будет использовано фактическое количество строк. |
| maxColumnCount | int | Ограничение количества столбцов в возвращаемом массиве. Если оно неположительное или превышает фактическое количество строк, будет использовано фактическое количество столбцов. |

**Returns:**
java.lang.Object[][] - Массив, который содержит все элементы, представленные указанным параметром.
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Получает объект Workbook, в котором находится функция.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Получает объект Worksheet, в котором находится функция.

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




### setCalculatedValue(Object value) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object value)
```


Устанавливает вычисленное значение для этой функции.

**Remarks**

Пользователь должен установить это свойство в своем пользовательском движке вычислений для тех функций, которые поддерживает движок, и установленное значение будет возвращено при последующем получении этого свойства. Установленное значение может быть одним из возможных типов: [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), массивом таких значений, или объектом Range, Name, ReferredArea. Получение этого свойства до установки значения приведет к вычислению функции движком вычислений по умолчанию Aspose.Cells, после чего будет возвращено вычисленное значение (обычно это будет \#NAME? для пользовательских функций).

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

