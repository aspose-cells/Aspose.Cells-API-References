---
title: "LookInType"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет тип «look in»."
type: docs
url: /ru/java/com.aspose.cells/lookintype/
---

**Inheritance:**
java.lang.Object
```
public final class LookInType
```

Представляет тип «look in».
## Поля

| Поле | Описание |
| --- | --- |
| [COMMENTS](#COMMENTS) | Находит объект только из комментария ячейки. |
| [FORMATTED_VALUES](#FORMATTED-VALUES) | Находит объект только из отформатированного значения ячейки ([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)). |
| [FORMULAS](#FORMULAS) | Находит искомый объект из формулы ([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)), если ячейка содержит формулу, иначе ищет из оригинального значения ячейки (то же, что и [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)). |
| [ONLY_FORMULAS](#ONLY-FORMULAS) | Игнорирует ячейки, которые не являются формулой. |
| [ORIGINAL_VALUES](#ORIGINAL-VALUES) | Найти объект только по исходному значению ячейки. |
| [VALUES](#VALUES) | Находит объект по исходному значению ячейки([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) и отформатированному значению([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)). |
| [VALUES_EXCLUDE_FORMULA_CELL](#VALUES-EXCLUDE-FORMULA-CELL) | Игнорирует ячейки, которые являются формулой. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### COMMENTS {#COMMENTS}
```
public static final int COMMENTS
```


Находит объект только по комментарию ячейки. Игнорирует ячейки без комментариев.

### FORMATTED_VALUES {#FORMATTED-VALUES}
```
public static final int FORMATTED_VALUES
```


Находит объект только из отформатированного значения ячейки ([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)).

### FORMULAS {#FORMULAS}
```
public static final int FORMULAS
```


Находит искомый объект из формулы ([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)), если ячейка содержит формулу, иначе ищет из оригинального значения ячейки (то же, что и [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)).

### ONLY_FORMULAS {#ONLY-FORMULAS}
```
public static final int ONLY_FORMULAS
```


Игнорирует ячейки, которые не являются формулой. Для ячеек, являющихся формулой, ищет искомый объект из формулы([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)).

### ORIGINAL_VALUES {#ORIGINAL-VALUES}
```
public static final int ORIGINAL_VALUES
```


Найти объект только по исходному значению ячейки.

### VALUES {#VALUES}
```
public static final int VALUES
```


Находит объект по исходному значению ячейки([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) и отформатированному значению([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)).

### VALUES_EXCLUDE_FORMULA_CELL {#VALUES-EXCLUDE-FORMULA-CELL}
```
public static final int VALUES_EXCLUDE_FORMULA_CELL
```


Игнорирует ячейки, которые являются формулой. Для ячеек, не являющихся формулой, используется то же, что и с [VALUES](../../com.aspose.cells/lookintype\#VALUES).

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

