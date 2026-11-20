---
title: "AbstractLowCodeLoadOptionsProvider"
second_title: "Справочник API Aspose.Cells for Java"
description: "Реализация, предоставляющая несколько вариантов загрузки для процессов, использующих несколько входных данных, таких как файлы шаблонов."
type: docs
url: /ru/java/com.aspose.cells/abstractlowcodeloadoptionsprovider/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractLowCodeLoadOptionsProvider
```

Реализация, предоставляющая несколько вариантов загрузки для процессов, использующих несколько входных данных (например, файлов шаблонов).

**Remarks**

Например, функция [SpreadsheetMerger](../../com.aspose.cells/spreadsheetmerger) требует нескольких файлов шаблонов для объединения.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [AbstractLowCodeLoadOptionsProvider()](#AbstractLowCodeLoadOptionsProvider--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeLoadOptions part)](#finish-com.aspose.cells.LowCodeLoadOptions-) | Освобождает ресурсы после обработки текущей части входных данных. |
| [getClass()](#getClass--) |  |
| [getCurrent()](#getCurrent--) | Получает параметры загрузки, из которых загружать данные текущей обрабатываемой части. |
| [hashCode()](#hashCode--) |  |
| [moveNext()](#moveNext--) | Проверяет, есть ли дополнительные входные данные. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeLoadOptionsProvider() {#AbstractLowCodeLoadOptionsProvider--}
```
public AbstractLowCodeLoadOptionsProvider()
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
### finish(LowCodeLoadOptions part) {#finish-com.aspose.cells.LowCodeLoadOptions-}
```
public void finish(LowCodeLoadOptions part)
```


Освобождает ресурсы после обработки текущей части входных данных.

**Remarks**

По умолчанию этот метод просто закрывает поток, указанный в [LowCodeLoadOptions.getInputStream()](../../com.aspose.cells/lowcodeloadoptions\#getInputStream--) напрямую (если параметры загрузки указали Stream как источник). Пользователь может переопределить этот метод, чтобы контролировать освобождение ресурсов в соответствии со своими требованиями и реализацией [getCurrent()](../../com.aspose.cells/abstractlowcodeloadoptionsprovider\#getCurrent--).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| part | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | параметры загрузки, используемые для текущей части. |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrent() {#getCurrent--}
```
public abstract LowCodeLoadOptions getCurrent()
```


Получает параметры загрузки, из которых загружать данные текущей обрабатываемой части.

**Returns:**
[LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### moveNext() {#moveNext--}
```
public abstract boolean moveNext()
```


Проверяет, есть ли дополнительные входные данные.

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

