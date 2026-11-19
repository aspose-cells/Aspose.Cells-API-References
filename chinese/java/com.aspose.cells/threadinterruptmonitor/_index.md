---
title: "ThreadInterruptMonitor"
second_title: "Aspose.Cells for Java API 参考"
description: "通过启动另一个线程，在睡眠用户指定的限制后要求中断的简单实现。"
type: docs
url: /zh/java/com.aspose.cells/threadinterruptmonitor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
```
public class ThreadInterruptMonitor extends AbstractInterruptMonitor
```

通过启动另一个线程，在睡眠用户指定的限制后要求中断的 [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) 的简单实现。

**Remarks**

一个监视器实例可以重复使用，只要按顺序监视每个过程。它不应在多线程中并发监视多个过程。

**Example**

以下示例展示了如何使用指定的时间限制来监控加载和保存过程：

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
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ThreadInterruptMonitor(boolean terminateWithoutException)](#ThreadInterruptMonitor-boolean-) | 构造一个中断监视器。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finishMonitor()](#finishMonitor--) | 结束对单个过程的监视。 |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | 参见 [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--)。 |
| [hashCode()](#hashCode--) |  |
| [isInterruptionRequested()](#isInterruptionRequested--) | 此实现仅检查时间消耗（从启动此监视器到现在的时间）是否大于用户指定的限制。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [startMonitor(int msLimit)](#startMonitor-int-) | 使用指定的时间限制启动监视器。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ThreadInterruptMonitor(boolean terminateWithoutException) {#ThreadInterruptMonitor-boolean-}
```
public ThreadInterruptMonitor(boolean terminateWithoutException)
```


构造一个中断监视器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| terminateWithoutException | boolean | [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--) |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### finishMonitor() {#finishMonitor--}
```
public void finishMonitor()
```


结束对单个过程的监视。

**Remarks**

在受监视的过程结束后调用此方法可以更早释放监视线程，尤其是当该过程没有中断（该过程的耗时小于指定的时间限制）时。

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


参见 [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--)。此属性在构造此监视器实例时由用户指定。

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


此实现仅检查时间消耗（从启动此监视器到现在的时间）是否大于用户指定的限制。

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


使用指定的时间限制启动监视器。计算时间消耗的起始时间即为调用此方法的时刻，因此需要监控的过程应在此调用后立即开始。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| msLimit | int | 中断所需的时间限制（毫秒）。 |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

