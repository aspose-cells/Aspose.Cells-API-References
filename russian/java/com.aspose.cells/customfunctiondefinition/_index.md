---
title: "CustomFunctionDefinition"
second_title: "Справочник API Aspose.Cells for Java"
description: "Определение пользовательской функции для вычислений с использованием пользовательского движка."
type: docs
url: /ru/java/com.aspose.cells/customfunctiondefinition/
---

**Inheritance:**
java.lang.Object
```
public class CustomFunctionDefinition
```

Определение пользовательской функции для вычислений с использованием пользовательского движка.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [CustomFunctionDefinition()](#CustomFunctionDefinition--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArrayModeParameters(String functionName)](#getArrayModeParameters-java.lang.String-) | Получает индексы параметров заданной пользовательской функции, которые необходимо вычислять в режиме массива. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomFunctionDefinition() {#CustomFunctionDefinition--}
```
public CustomFunctionDefinition()
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
### getArrayModeParameters(String functionName) {#getArrayModeParameters-java.lang.String-}
```
public int[] getArrayModeParameters(String functionName)
```


Получает индексы параметров заданной пользовательской функции, которые необходимо вычислять в режиме массива.

**Remarks**

Для выражения, которое необходимо вычислить, беря в качестве примера A:A+B:B: Обычно в режиме значения оно будет вычислено в единственное значение в соответствии с текущей ячейкой. Но в режиме массива все значения A1+B1, A2+B2, A3+B3, ... будут вычислены и использованы для расчёта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| functionName | java.lang.String | Имя пользовательской функции. |

**Returns:**
int[] — Индексы параметров, которые необходимо вычислять в режиме массива для заданной пользовательской функции. По умолчанию null, нет параметров, требующих вычисления в режиме массива для этой функции.
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

