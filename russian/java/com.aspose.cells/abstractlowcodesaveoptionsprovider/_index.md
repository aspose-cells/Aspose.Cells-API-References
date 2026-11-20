---
title: "AbstractLowCodeSaveOptionsProvider"
second_title: "Справочник API Aspose.Cells for Java"
description: "Реализация, предоставляющая несколько вариантов сохранения для процессов, требующих несколько выходных данных."
type: docs
url: /ru/java/com.aspose.cells/abstractlowcodesaveoptionsprovider/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractLowCodeSaveOptionsProvider
```

Реализация, предоставляющая несколько вариантов сохранения для процессов, требующих множественных выходов. Например, функция [SpreadsheetSplitter](../../com.aspose.cells/spreadsheetsplitter) требует нескольких назначений для сохранения разделённых файлов.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [AbstractLowCodeSaveOptionsProvider()](#AbstractLowCodeSaveOptionsProvider--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Освобождает ресурсы после обработки текущей части разделения. |
| [getClass()](#getClass--) |  |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Получает параметры сохранения, из которых берутся настройки вывода для текущей части разделения. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeSaveOptionsProvider() {#AbstractLowCodeSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider()
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
### finish(LowCodeSaveOptions part) {#finish-com.aspose.cells.LowCodeSaveOptions-}
```
public void finish(LowCodeSaveOptions part)
```


Освобождает ресурсы после обработки текущей части разделения.

**Remarks**

По умолчанию этот метод просто закрывает поток, указанный в [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--), напрямую (если параметры сохранения указали поток в качестве назначения). Пользователь может переопределить этот метод, чтобы управлять освобождением ресурсов в соответствии со своими требованиями и реализацией [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| part | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | параметры сохранения, используемые для текущей части разделения. |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public abstract LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```


Получает параметры сохранения, из которых берутся настройки вывода для текущей части разделения. Возврат null означает пропустить данную часть.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
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

