---
title: "ThreadInterruptMonitor"
second_title: "Справочник API Aspose.Cells for Java"
description: "Простая реализация  путем запуска другого потока, требующего прерывания после ожидания указанного пользователем предела."
type: docs
url: /ru/java/com.aspose.cells/threadinterruptmonitor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
```
public class ThreadInterruptMonitor extends AbstractInterruptMonitor
```

Простая реализация [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) путем запуска другого потока, требующего прерывания после ожидания указанного пользователем предела.

**Remarks**

Один экземпляр монитора можно использовать многократно, при условии, что вы отслеживаете каждый процесс последовательно. Его не следует использовать для одновременного мониторинга нескольких процедур в многопоточной среде.

**Example**

Следующий пример показывает, как контролировать процесс загрузки и сохранения с указанным ограничением времени:

```
         ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
         LoadOptions lopts = new LoadOptions();
         lopts.setInterruptMonitor(monitor);
         monitor.startMonitor(1000); //time limit is 1 second
         Workbook wb = new Workbook("Large.xlsx", lopts);
         //if the time cost of loading the template file exceeds one second, interruption will be required and exception will be thrown here
         //otherwise finishes the monitor thread and starts to monitor the save procedure
         monitor.finishMonitor();
         monitor.startMonitor(1500); //time limit is 1.5 seconds
         wb.save("result.xlsx");
         monitor.finishMonitor();
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ThreadInterruptMonitor(boolean terminateWithoutException)](#ThreadInterruptMonitor-boolean-) | Создаёт один монитор прерываний. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finishMonitor()](#finishMonitor--) | Завершает монитор для одной процедуры. |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | См. [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). |
| [hashCode()](#hashCode--) |  |
| [isInterruptionRequested()](#isInterruptionRequested--) | Эта реализация просто проверяет, превышает ли затраченное время (от момента запуска этого монитора до текущего момента) заданное пользователем ограничение. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [startMonitor(int msLimit)](#startMonitor-int-) | Запускает монитор с указанным ограничением времени. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ThreadInterruptMonitor(boolean terminateWithoutException) {#ThreadInterruptMonitor-boolean-}
```
public ThreadInterruptMonitor(boolean terminateWithoutException)
```


Создаёт один монитор прерываний.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| terminateWithoutException | boolean | [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--) |

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
### finishMonitor() {#finishMonitor--}
```
public void finishMonitor()
```


Завершает монитор для одной процедуры.

**Remarks**

Вызов этого метода после мониторируемой процедуры может освободить поток монитора раньше, особенно когда для неё нет прерываний (время выполнения этой процедуры меньше указанного предела).

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


См. [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). Это свойство задаётся пользователем при создании экземпляра этого монитора.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isInterruptionRequested() {#isInterruptionRequested--}
```
public boolean isInterruptionRequested()
```


Эта реализация просто проверяет, превышает ли затраченное время (от момента запуска этого монитора до текущего момента) заданное пользователем ограничение.

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




### startMonitor(int msLimit) {#startMonitor-int-}
```
public void startMonitor(int msLimit)
```


Запускает монитор с указанным ограничением времени. Время начала для расчёта затрат времени фиксируется в момент вызова этого метода, поэтому процедура, которую необходимо отслеживать, должна быть запущена сразу после этого вызова.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| msLimit | int | ограничение времени (мс) для требуемого прерывания. |

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

