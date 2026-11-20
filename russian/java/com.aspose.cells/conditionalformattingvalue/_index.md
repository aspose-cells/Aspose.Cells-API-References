---
title: "ConditionalFormattingValue"
second_title: "Справочник API Aspose.Cells for Java"
description: "Описывает значения точек интерполяции в градиентной шкале dataBar или iconSet."
type: docs
url: /ru/java/com.aspose.cells/conditionalformattingvalue/
---

**Inheritance:**
java.lang.Object
```
public class ConditionalFormattingValue
```

Описывает значения точек интерполяции в градиентной шкале, полосе данных или наборе значков.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Получает тип этого объекта значения условного форматирования. |
| [getValue()](#getValue--) | Получает значение этого объекта значения условного форматирования. |
| [hashCode()](#hashCode--) |  |
| [isGTE()](#isGTE--) | Получает флаг «Больше или равно». |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setGTE(boolean value)](#setGTE-boolean-) | Устанавливает флаг «Больше или равно». |
| [setType(int value)](#setType-int-) | Устанавливает тип этого объекта значения условного форматирования. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Устанавливает значение этого объекта значения условного форматирования. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getType() {#getType--}
```
public int getType()
```


Получает тип этого объекта значения условного форматирования. Установка типа в FormatConditionValueType.Min или FormatConditionValueType.Max автоматически задаст "Value" равным null.

Смотрите [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Получает значение этого объекта значения условного форматирования. Должно использоваться вместе с Type.

**Remarks**

Если значение является строкой и начинается с "=", оно будет обработано как формула, иначе будет обработано как простое значение.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGTE() {#isGTE--}
```
public boolean isGTE()
```


Получает флаг «Больше или равно». Используется только для наборов значков, определяет, использует ли это пороговое значение оператор «больше или равно». 'false' указывает, что используется «больше», а не «больше или равно». Значение по умолчанию — true.

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




### setGTE(boolean value) {#setGTE-boolean-}
```
public void setGTE(boolean value)
```


Устанавливает флаг «Больше или равно». Используется только для наборов значков, определяет, использует ли это пороговое значение оператор «больше или равно». 'false' указывает, что используется «больше», а не «больше или равно». Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Устанавливает тип этого объекта значения условного форматирования. Установка типа в FormatConditionValueType.Min или FormatConditionValueType.Max автоматически задаст "Value" равным null.

Смотрите [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Устанавливает значение этого объекта значения условного форматирования. Должно использоваться вместе с Type.

**Remarks**

Если значение является строкой и начинается с "=", оно будет обработано как формула, иначе будет обработано как простое значение.

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

