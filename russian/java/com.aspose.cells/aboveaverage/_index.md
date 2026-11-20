---
title: "AboveAverage"
second_title: "Справочник API Aspose.Cells for Java"
description: "Опишите правило условного форматирования AboveAverage."
type: docs
url: /ru/java/com.aspose.cells/aboveaverage/
---

**Inheritance:**
java.lang.Object
```
public class AboveAverage
```

Опишите правило условного форматирования AboveAverage. Это правило условного форматирования выделяет ячейки, которые находятся выше или ниже среднего значения для всех значений в диапазоне.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [AboveAverage()](#AboveAverage--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getStdDev()](#getStdDev--) | Получает количество стандартных отклонений, включаемых выше или ниже среднего в правиле условного форматирования. |
| [hashCode()](#hashCode--) |  |
| [isAboveAverage()](#isAboveAverage--) | Получает флаг, указывающий, является ли правило правилом "above average". |
| [isEqualAverage()](#isEqualAverage--) | Получает флаг, указывающий, включают ли критерии 'aboveAverage' и 'belowAverage' само среднее значение или исключают его. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAboveAverage(boolean value)](#setAboveAverage-boolean-) | Устанавливает флаг, указывающий, является ли правило правилом "above average". |
| [setEqualAverage(boolean value)](#setEqualAverage-boolean-) | Устанавливает флаг, указывающий, включают ли критерии 'aboveAverage' и 'belowAverage' само среднее значение или исключают его. |
| [setStdDev(int value)](#setStdDev-int-) | Устанавливает количество стандартных отклонений, включаемых выше или ниже среднего в правиле условного форматирования. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AboveAverage() {#AboveAverage--}
```
public AboveAverage()
```


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
### getStdDev() {#getStdDev--}
```
public int getStdDev()
```


Получает количество стандартных отклонений, включаемых выше или ниже среднего в правиле условного форматирования. Входное значение должно быть от 0 до 3 (включительно). Установка этого значения в 0 означает, что stdDev не задан. Значение по умолчанию — 0.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAboveAverage() {#isAboveAverage--}
```
public boolean isAboveAverage()
```


Получает флаг, указывающий, является ли правило \"above average\". 'true' означает 'above average'. Значение по умолчанию — true.

**Returns:**
boolean
### isEqualAverage() {#isEqualAverage--}
```
public boolean isEqualAverage()
```


Получает флаг, указывающий, включают ли критерии 'aboveAverage' и 'belowAverage' само среднее значение или исключают его. 'true' означает включить среднее значение в критерий. Значение по умолчанию — false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAboveAverage(boolean value) {#setAboveAverage-boolean-}
```
public void setAboveAverage(boolean value)
```


Устанавливает флаг, указывающий, является ли правило \"above average\". 'true' означает 'above average'. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEqualAverage(boolean value) {#setEqualAverage-boolean-}
```
public void setEqualAverage(boolean value)
```


Устанавливает флаг, указывающий, включают ли критерии 'aboveAverage' и 'belowAverage' само среднее значение или исключают его. 'true' означает включить среднее значение в критерий. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setStdDev(int value) {#setStdDev-int-}
```
public void setStdDev(int value)
```


Устанавливает количество стандартных отклонений, включаемых выше или ниже среднего в правиле условного форматирования. Входное значение должно быть от 0 до 3 (включительно). Установка этого значения в 0 означает, что stdDev не задан. Значение по умолчанию — 0.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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

