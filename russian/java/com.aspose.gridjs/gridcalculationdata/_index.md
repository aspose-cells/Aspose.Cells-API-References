---
title: "GridCalculationData"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет необходимые данные при вычислении функции, таких как имя функции, параметры … и т.д."
type: docs
url: /ru/java/com.aspose.gridjs/gridcalculationdata/
---

**Inheritance:**
java.lang.Object
```
public class GridCalculationData
```

Представляет необходимые данные при вычислении функции, такие как имя функции, параметры и т.д.

**Remarks**

Все объекты, предоставляемые этим классом, предназначены только для "read". Пользователь не должен изменять какие-либо данные в Workbook во время процесса вычисления формул, иначе могут возникнуть неожиданные результаты или Exception.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Получает вычисленное значение этой функции. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Получает индекс столбца Cell, в которой находится функция. |
| [getFormula()](#getFormula--) | Получает формулу Cell, в которой находится функция. |
| [getFunctionName()](#getFunctionName--) | Получает имя функции, которую нужно вычислить. |
| [getParamCount()](#getParamCount--) | Получает количество параметров. |
| [getParamText(int index)](#getParamText-int-) | Получает буквальный текст параметра по заданному индексу. |
| [getParamValue(int index)](#getParamValue-int-) | Получает представленный объект значения параметра по заданному индексу. |
| [getRow()](#getRow--) | Получает индекс строки Cell, в которой находится функция. |
| [getSheetName()](#getSheetName--) | Получает имя листа, в котором находится функция. |
| [getStringValue()](#getStringValue--) | Получает DisplayStringValue ячейки Cell, в которой находится функция. |
| [getValue()](#getValue--) | Получает значение ячейки Cell, в которой находится функция. |
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

Пользователь должен установить это свойство в своем пользовательском движке вычислений для тех функций, которые поддерживает движок, и установленное значение будет возвращено при получении этого свойства. Получение этого свойства до его установки приведет к вычислению функции движком вычислений по умолчанию Aspose.Cells, и будет возвращено вычисленное значение.

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Получает индекс столбца Cell, в которой находится функция.

**Returns:**
int
### getFormula() {#getFormula--}
```
public String getFormula()
```


Получает формулу Cell, в которой находится функция.

**Returns:**
java.lang.String
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


Получает количество параметров.

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
| индекс | int | Индекс параметра (начиная с 0). |

**Returns:**
java.lang.String - Буквальный текст параметра.
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


Получает представленный объект значения параметра по заданному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс параметра (начиная с 0). |

**Returns:**
java.lang.Object - Если параметр является простым значением, то возвращает простое значение. Если параметр является ссылкой, то возвращает объект ReferredArea.
### getRow() {#getRow--}
```
public int getRow()
```


Получает индекс строки Cell, в которой находится функция.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Получает имя листа, в котором находится функция.

**Returns:**
java.lang.String
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Получает DisplayStringValue ячейки Cell, в которой находится функция.

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


Получает значение ячейки Cell, в которой находится функция.

**Returns:**
java.lang.Object
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

Пользователь должен установить это свойство в своем пользовательском движке вычислений для тех функций, которые поддерживает движок, и установленное значение будет возвращено при получении этого свойства. Получение этого свойства до его установки приведет к вычислению функции движком вычислений по умолчанию Aspose.Cells, и будет возвращено вычисленное значение.

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

