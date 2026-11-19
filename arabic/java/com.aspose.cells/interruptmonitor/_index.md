---
title: "InterruptMonitor"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل جميع المشغلات المتعلقة بالمقاطعة."
type: docs
url: /ar/java/com.aspose.cells/interruptmonitor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
```
public class InterruptMonitor extends AbstractInterruptMonitor
```

يمثل جميع المشغلات المتعلقة بالمقاطعة.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [InterruptMonitor()](#InterruptMonitor--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | عند انقطاع الإجراء، ما إذا كان يجب إنهاء الإجراء بهدوء أم رمي استثناء. |
| [hashCode()](#hashCode--) |  |
| [interrupt()](#interrupt--) | قاطع المشغل الحالي. |
| [isInterruptionRequested()](#isInterruptionRequested--) | ضع علامة على المراقب كطالب بالانقطاع |
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
| معامل | نوع | الوصف |
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


عند انقطاع الإجراء، سواء إنهاء الإجراء بهدوء أو رمي استثناء. القيمة الافتراضية هي false، أي عندما يكون [isInterruptionRequested()](../../com.aspose.cells/abstractinterruptmonitor\#isInterruptionRequested--) صحيحًا، سيتم رمي [CellsException](../../com.aspose.cells/cellsexception) بالرمز [ExceptionType.INTERRUPTED](../../com.aspose.cells/exceptiontype\#INTERRUPTED).

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


قاطع المشغل الحالي.

### isInterruptionRequested() {#isInterruptionRequested--}
```
public boolean isInterruptionRequested()
```


ضع علامة على المراقب كطالب بالانقطاع

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

