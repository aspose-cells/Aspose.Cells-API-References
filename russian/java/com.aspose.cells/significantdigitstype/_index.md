---
title: "SignificantDigitsType"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет тип значимых цифр для вывода числовых значений."
type: docs
url: /ru/java/com.aspose.cells/significantdigitstype/
---

**Inheritance:**
java.lang.Object
```
public final class SignificantDigitsType
```

Представляет тип значимых цифр для вывода числовых значений.
## Поля

| Поле | Описание |
| --- | --- |
| [DIGITS_15](#DIGITS-15) | 15 знаков |
| [G_17](#G-17) | 17 знаков при форматировании значения с помощью \"G17\". |
| [ROUNDING_17](#ROUNDING-17) | 17 знаков при округлении значения. |
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
### DIGITS_15 {#DIGITS-15}
```
public static final int DIGITS_15
```


15 знаков

### G_17 {#G-17}
```
public static final int G_17
```


17 знаков при форматировании значения с помощью \"G17\".

**Remarks**

Для некоторых значений типа double, \"G17\" может возвращать другое значение, чем исходное/литеральное, введённое пользователем. Например, значение double 0.15 будет выведено как 0.14999999999999999; значение double 1.0E-16 будет выведено как 9.9999999999999998E-17. Excel от Microsoft обрабатывает эти значения непоследовательно: он сохраняет 0.15 как 0.15 в файле xlsx, но для 1.0E-16 сохранённое значение в файле xlsx равно 9.9999999999999998E-17.

### ROUNDING_17 {#ROUNDING-17}
```
public static final int ROUNDING_17
```


17 знаков при округлении значения.

**Remarks**

Этот тип обычно выводит значение как исходное/литеральное, введённое пользователем. Для 0.15 он выдаёт \"0.15\", а для 1.0E-16 — \"1.0E-16\". Однако существуют специальные случаи, когда могут получаться значения, отличные от литеральных. Например, при округлении 208435494.96478021 до 17 знаков (\"0.\\#\\#\\#\\#\\#\\#\\#\\#\\#\\#\\#\\#\\#\\#\\#\\#\"), результатом будет 208435494.96478.

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

