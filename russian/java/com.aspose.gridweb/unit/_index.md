---
title: "Unit"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет измерение длины"
type: docs
url: /ru/java/com.aspose.gridweb/unit/
---

**Inheritance:**
java.lang.Object
```
public class Unit
```

Представляет измерение длины
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Unit()](#Unit--) | конструктор по умолчанию |
| [Unit(double value, int type)](#Unit-double-int-) | Инициализирует новый экземпляр структуры Unit с указанным числом двойной точности и типом UnitType. |
| [Unit(double value)](#Unit-double-) | Инициализирует новый экземпляр структуры Unit с указанным числом двойной точности. |
| [Unit(int value)](#Unit-int-) | Инициализирует новый экземпляр структуры Unit с указанным 32‑битным знаковым целым числом. |
| [Unit(String value)](#Unit-java.lang.String-) | Инициализирует новый экземпляр структуры Unit с указанной длиной. |
## Методы

| Метод | Описание |
| --- | --- |
| [GetExtension(int type)](#GetExtension-int-) | получить строку по типу, может вернуть "px", "pt", "%" и т.д.; |
| [Parse(String s)](#Parse-java.lang.String-) | Преобразует указанную строку в Unit. |
| [Percentage(double n)](#Percentage-double-) | Создаёт Unit типа Percentage из указанного числа двойной точности. |
| [Pixel(int n)](#Pixel-int-) | Создаёт Unit типа Pixel из указанного 32‑битного знакового целого числа. |
| [Point(int n)](#Point-int-) | Создаёт Unit типа Point из указанного 32‑битного знакового целого числа. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Возвращает тип единицы Unit. |
| [getValue()](#getValue--) | Возвращает длину Unit. |
| [hashCode()](#hashCode--) |  |
| [isEmpty()](#isEmpty--) | Возвращает значение, указывающее, пустой ли Unit. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | получить строковое представление единицы. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Unit() {#Unit--}
```
public Unit()
```


конструктор по умолчанию

### Unit(double value, int type) {#Unit-double-int-}
```
public Unit(double value, int type)
```


Инициализирует новый экземпляр структуры Unit с указанным числом двойной точности и типом UnitType.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |
| тип | int |  |

### Unit(double value) {#Unit-double-}
```
public Unit(double value)
```


Инициализирует новый экземпляр структуры Unit с указанным числом двойной точности.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### Unit(int value) {#Unit-int-}
```
public Unit(int value)
```


Инициализирует новый экземпляр структуры Unit с указанным 32‑битным знаковым целым числом.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### Unit(String value) {#Unit-java.lang.String-}
```
public Unit(String value)
```


Инициализирует новый экземпляр структуры Unit с указанной длиной.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### GetExtension(int type) {#GetExtension-int-}
```
public static String GetExtension(int type)
```


получить строку по типу, может вернуть "px", "pt", "%" и т.д.;

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| тип | int |  |

**Returns:**
java.lang.String
### Parse(String s) {#Parse-java.lang.String-}
```
public static Unit Parse(String s)
```


Преобразует указанную строку в Unit.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| s | java.lang.String |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Percentage(double n) {#Percentage-double-}
```
public static Unit Percentage(double n)
```


Создаёт Unit типа Percentage из указанного числа двойной точности.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| n | double |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Pixel(int n) {#Pixel-int-}
```
public static Unit Pixel(int n)
```


Создаёт Unit типа Pixel из указанного 32‑битного знакового целого числа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Point(int n) {#Point-int-}
```
public static Unit Point(int n)
```


Создаёт Unit типа Point из указанного 32‑битного знакового целого числа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
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


Возвращает тип единицы Unit.

**Returns:**
int
### getValue() {#getValue--}
```
public double getValue()
```


Возвращает длину Unit.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Возвращает значение, указывающее, пустой ли Unit.

**Returns:**
boolean -
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


получить строковое представление единицы.

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

