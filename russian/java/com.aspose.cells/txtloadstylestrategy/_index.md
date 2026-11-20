---
title: "TxtLoadStyleStrategy"
second_title: "Справочник API Aspose.Cells for Java"
description: "Указывает, как применять стиль к разобранным значениям при преобразовании строкового значения в число или дату/время."
type: docs
url: /ru/java/com.aspose.cells/txtloadstylestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class TxtLoadStyleStrategy
```

Указывает, как применять стиль к разобранным значениям при преобразовании строкового значения в число или дату/время.
## Поля

| Поле | Описание |
| --- | --- |
| [BUILT_IN](#BUILT-IN) | Установите стиль как встроенный номер/дата‑время, когда разобранное значение является простым числовым/датовым значением. |
| [EXACT_FORMAT](#EXACT-FORMAT) | Установите точный пользовательский формат для разобранного значения, чтобы отформатированное значение было таким же, как исходный ввод. |
| [NONE](#NONE) | Не устанавливает стиль для разобранного значения. |
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
### BUILT_IN {#BUILT-IN}
```
public static final int BUILT_IN
```


Установите стиль как встроенный номер/дата‑время, когда разобранное значение является простым числовым/датовым значением.

**Remarks**

Когда MS Excel разбирает значения даты/времени или числовые значения в соответствии с вводом пользователя (например, CSV‑файл), форматирование этих значений может измениться, например, ведущие/конечные нули числа, порядок год/месяц/день даты/времени и т.д. Этот тип предназначен для имитации поведения MS Excel.

### EXACT_FORMAT {#EXACT-FORMAT}
```
public static final int EXACT_FORMAT
```


Установите точный пользовательский формат для разобранного значения, чтобы отформатированное значение было таким же, как исходный ввод.

### NONE {#NONE}
```
public static final int NONE
```


Не устанавливает стиль для разобранного значения.

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

