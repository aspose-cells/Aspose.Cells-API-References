---
title: "AbstractInterruptMonitor"
second_title: "Aspose.Cells for Java API 参考"
description: "监视所有耗时操作中的中断请求。"
type: docs
url: /zh/java/com.aspose.cells/abstractinterruptmonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractInterruptMonitor
```

监视所有耗时操作中的中断请求。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AbstractInterruptMonitor()](#AbstractInterruptMonitor--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | 当过程被中断时，是安静地终止过程还是抛出异常。 |
| [hashCode()](#hashCode--) |  |
| [isInterruptionRequested()](#isInterruptionRequested--) | 指示当前操作是否已请求中断。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractInterruptMonitor() {#AbstractInterruptMonitor--}
```
public AbstractInterruptMonitor()
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
### isInterruptionRequested() {#isInterruptionRequested--}
```
public abstract boolean isInterruptionRequested()
```


指示是否为当前操作请求中断。如果为 true，则当前操作将被中断。实现应在此进行快速高效的检查，否则可能成为过程的另一个瓶颈。

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

