---
title: "AbstractInterruptMonitor"
second_title: "Aspose.Cells for Java API Reference"
description: "مراقبة لطلبات الإيقاف في جميع العمليات المستهلكة للوقت."
type: docs
url: /ar/java/com.aspose.cells/abstractinterruptmonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractInterruptMonitor
```

مراقبة لطلبات الإيقاف في جميع العمليات المستهلكة للوقت.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [AbstractInterruptMonitor()](#AbstractInterruptMonitor--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | عند انقطاع الإجراء، ما إذا كان يجب إنهاء الإجراء بهدوء أم رمي استثناء. |
| [hashCode()](#hashCode--) |  |
| [isInterruptionRequested()](#isInterruptionRequested--) | يشير إلى ما إذا كان تم طلب الانقطاع للعملية الحالية. |
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
### isInterruptionRequested() {#isInterruptionRequested--}
```
public abstract boolean isInterruptionRequested()
```


يشير إلى ما إذا كان تم طلب الانقطاع للعملية الحالية. إذا كان صحيحًا فستتوقف العملية الحالية. يجب على التنفيذ إجراء فحص سريع وفعال هنا، وإلا قد يصبح عنق زجاجة آخر للإجراء.

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

