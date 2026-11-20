---
title: "SplitPartInfo"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет информацию одного входа/выхода для множественных входов/выходов, например текущей страницы, которая будет отрисована при преобразовании таблицы в изображение."
type: docs
url: /ru/java/com.aspose.cells/splitpartinfo/
---

**Inheritance:**
java.lang.Object
```
public class SplitPartInfo
```

Представляет информацию об одном вводе/выводе для множественных вводов/выводов, например текущей странице, которая будет отрисована при преобразовании таблицы в изображение.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPartIndex()](#getPartIndex--) | Индекс текущей части в последовательности (нумерация с нуля). |
| [getSheetIndex()](#getSheetIndex--) | Индекс листа, в котором находится текущая часть. -1 обозначает, что лист единственный. |
| [getSheetName()](#getSheetName--) | Имя листа, в котором находится текущая часть. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
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
### getPartIndex() {#getPartIndex--}
```
public int getPartIndex()
```


Индекс текущей части в последовательности (нумерация с нуля). -1 означает, что нет нескольких частей, поэтому результат единственный.

**Remarks**

Если необходимо обработать несколько листов и каждый лист обрабатывается (разделяется) отдельно, индекс части всегда начинается с 0 для каждого листа. Например, при преобразовании книги в изображения это представляет индекс выходной страницы текущего обрабатываемого листа. А -1 обозначает, что для текущего листа есть только одна страница.

**Returns:**
int
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


Индекс листа, в котором находится текущая часть. -1 обозначает, что лист единственный.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Имя листа, в котором находится текущая часть.

**Remarks**

Может быть null в некоторых ситуациях, например при рендеринге всей книги в TIFF‑изображение.

**Returns:**
java.lang.String
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

