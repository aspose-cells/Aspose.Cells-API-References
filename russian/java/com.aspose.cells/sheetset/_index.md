---
title: "SheetSet"
second_title: "Справочник API Aspose.Cells for Java"
description: "Описывает набор листов."
type: docs
url: /ru/java/com.aspose.cells/sheetset/
---

**Inheritance:**
java.lang.Object
```
public class SheetSet
```

Описывает набор листов.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SheetSet(int[] sheetIndexes)](#SheetSet-int---) | Создаёт набор листов на основе точных индексов листов. |
| [SheetSet(String[] sheetNames)](#SheetSet-java.lang.String---) | Создаёт набор листов на основе точных имён листов. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActive()](#getActive--) | Получает набор с активным листом книги. |
| [getAll()](#getAll--) | Получает набор со всеми листами книги в их исходном порядке. |
| [getClass()](#getClass--) |  |
| [getVisible()](#getVisible--) | Получает набор с видимыми листами книги в их исходном порядке. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetSet(int[] sheetIndexes) {#SheetSet-int---}
```
public SheetSet(int[] sheetIndexes)
```


Создаёт набор листов на основе точных индексов листов.

**Remarks**

Если встречается лист, которого нет в книге, во время рендеринга будет выброшено исключение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndexes | int[] | нумерация листов начинается с нуля. |

### SheetSet(String[] sheetNames) {#SheetSet-java.lang.String---}
```
public SheetSet(String[] sheetNames)
```


Создаёт набор листов на основе точных имён листов.

**Remarks**

Если встречается лист, которого нет в книге, во время рендеринга будет выброшено исключение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetNames | java.lang.String[] | имена листов. |

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
### getActive() {#getActive--}
```
public static SheetSet getActive()
```


Получает набор с активным листом книги.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getAll() {#getAll--}
```
public static SheetSet getAll()
```


Получает набор со всеми листами книги в их исходном порядке.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getVisible() {#getVisible--}
```
public static SheetSet getVisible()
```


Получает набор с видимыми листами книги в их исходном порядке.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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

