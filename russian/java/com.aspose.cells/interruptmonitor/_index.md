---
title: "InterruptMonitor"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет все операторы, связанные с прерыванием."
type: docs
url: /ru/java/com.aspose.cells/interruptmonitor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
```
public class InterruptMonitor extends AbstractInterruptMonitor
```

Представляет все операторы, связанные с прерыванием.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [InterruptMonitor()](#InterruptMonitor--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | Когда процедура прерывается, следует ли тихо завершить её или бросить исключение. |
| [hashCode()](#hashCode--) |  |
| [interrupt()](#interrupt--) | Прерывает текущий оператор. |
| [isInterruptionRequested()](#isInterruptionRequested--) | Помечает монитор как запрашивающий прерывание. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### InterruptMonitor() {#InterruptMonitor--}
```
public InterruptMonitor()
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
### getTerminateWithoutException() {#getTerminateWithoutException--}
```
public boolean getTerminateWithoutException()
```


Когда процедура прерывается, следует ли завершать её тихо или бросать исключение. По умолчанию false, то есть когда [isInterruptionRequested()](../../com.aspose.cells/abstractinterruptmonitor\#isInterruptionRequested--) истинно, будет выброшено [CellsException](../../com.aspose.cells/cellsexception) с кодом [ExceptionType.INTERRUPTED](../../com.aspose.cells/exceptiontype\#INTERRUPTED).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### interrupt() {#interrupt--}
```
public void interrupt()
```


Прерывает текущий оператор.

### isInterruptionRequested() {#isInterruptionRequested--}
```
public boolean isInterruptionRequested()
```


Помечает монитор как запрашивающий прерывание.

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

