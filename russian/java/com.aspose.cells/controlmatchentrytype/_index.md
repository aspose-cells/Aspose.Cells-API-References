---
title: "ControlMatchEntryType"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет способ, которым ListBox или ComboBox ищет в списке во время ввода пользователем."
type: docs
url: /ru/java/com.aspose.cells/controlmatchentrytype/
---

**Inheritance:**
java.lang.Object
```
public final class ControlMatchEntryType
```

Представляет способ, которым ListBox или ComboBox ищет в списке во время ввода пользователем.
## Поля

| Поле | Описание |
| --- | --- |
| [COMPLETE](#COMPLETE) | По мере ввода каждого символа контрол ищет запись, соответствующую всем введённым символам. |
| [FIRST_LETTER](#FIRST-LETTER) | Контрол ищет следующую запись, начинающуюся с введённого символа. |
| [NONE](#NONE) | Список не будет просматриваться при вводе символов. |
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
### COMPLETE {#COMPLETE}
```
public static final int COMPLETE
```


По мере ввода каждого символа контрол ищет запись, соответствующую всем введённым символам.

### FIRST_LETTER {#FIRST-LETTER}
```
public static final int FIRST_LETTER
```


Контрол ищет следующую запись, начинающуюся с введённого символа. При многократном вводе одной и той же буквы происходит переключение между всеми записями, начинающимися с этой буквы.

### NONE {#NONE}
```
public static final int NONE
```


Список не будет просматриваться при вводе символов.

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

