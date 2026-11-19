---
title: "InterruptMonitor"
second_title: "Aspose.Cells for Java API 参考"
description: "表示所有关于中断的操作符。"
type: docs
url: /zh/java/com.aspose.cells/interruptmonitor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
```
public class InterruptMonitor extends AbstractInterruptMonitor
```

表示所有关于中断的操作符。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [InterruptMonitor()](#InterruptMonitor--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | 当过程被中断时，是安静地终止过程还是抛出异常。 |
| [hashCode()](#hashCode--) |  |
| [interrupt()](#interrupt--) | 中断当前操作符。 |
| [isInterruptionRequested()](#isInterruptionRequested--) | 将监视器标记为请求中断 |
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
| 参数 | 类型 | 描述 |
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


当过程被中断时，是安静终止过程还是抛出异常。默认值为 false，即当 [isInterruptionRequested()](../../com.aspose.cells/abstractinterruptmonitor\#isInterruptionRequested--) 为 true，将抛出带有代码 [ExceptionType.INTERRUPTED](../../com.aspose.cells/exceptiontype\#INTERRUPTED) 的 [CellsException](../../com.aspose.cells/cellsexception)。

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


中断当前操作符。

### isInterruptionRequested() {#isInterruptionRequested--}
```
public boolean isInterruptionRequested()
```


将监视器标记为请求中断

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

