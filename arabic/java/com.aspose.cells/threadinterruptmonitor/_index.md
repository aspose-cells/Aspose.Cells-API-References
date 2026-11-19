---
title: "ThreadInterruptMonitor"
second_title: "Aspose.Cells for Java API Reference"
description: "تنفيذ بسيط لـ  عن طريق بدء خيط آخر لطلب المقاطعة بعد النوم للحد المحدد من قبل المستخدم."
type: docs
url: /ar/java/com.aspose.cells/threadinterruptmonitor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
```
public class ThreadInterruptMonitor extends AbstractInterruptMonitor
```

تنفيذ بسيط لـ [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) عن طريق بدء خيط آخر لطلب المقاطعة بعد النوم للحد المحدد من قبل المستخدم.

**Remarks**

يمكن استخدام نسخة مراقب واحدة بشكل متكرر، طالما أنك تراقب كل عملية بالتسلسل. لا ينبغي استخدامها لمراقبة إجراءات متعددة في وقت واحد عبر خيوط متعددة.

**Example**

المثال التالي يوضح كيفية مراقبة عملية التحميل والحفظ بحد زمني محدد:

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
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ThreadInterruptMonitor(boolean terminateWithoutException)](#ThreadInterruptMonitor-boolean-) | ينشئ مراقب مقاطعة واحد. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finishMonitor()](#finishMonitor--) | ينهي المراقب لإجراء واحد. |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | انظر [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). |
| [hashCode()](#hashCode--) |  |
| [isInterruptionRequested()](#isInterruptionRequested--) | هذا التنفيذ يتحقق فقط مما إذا كانت تكلفة الوقت (من لحظة بدء هذا المراقب حتى الآن) أكبر من الحد المحدد من قبل المستخدم. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [startMonitor(int msLimit)](#startMonitor-int-) | يبدأ المراقب بالحد الزمني المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ThreadInterruptMonitor(boolean terminateWithoutException) {#ThreadInterruptMonitor-boolean-}
```
public ThreadInterruptMonitor(boolean terminateWithoutException)
```


ينشئ مراقب مقاطعة واحد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| terminateWithoutException | boolean | [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--) |

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
### finishMonitor() {#finishMonitor--}
```
public void finishMonitor()
```


ينهي المراقب لإجراء واحد.

**Remarks**

استدعاء هذه الطريقة بعد الإجراء المراقَب يمكن أن يحرّر خيط المراقبة مبكرًا، خاصةً عندما لا يكون هناك انقطاع له (تكلفة الوقت لهذا الإجراء أقل من الحد الزمني المحدد).

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


انظر [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). يتم تحديد هذه الخاصية من قبل المستخدم عند إنشاء مثيل هذا المراقب.

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


هذا التنفيذ يتحقق فقط مما إذا كانت تكلفة الوقت (من لحظة بدء هذا المراقب حتى الآن) أكبر من الحد المحدد من قبل المستخدم.

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


يبدأ المراقب بالحد الزمني المحدد. وقت البدء لحساب تكلفة الوقت هو فقط عند استدعاء هذه الطريقة، لذا يجب بدء العملية التي تحتاج إلى المراقبة مباشرةً بعد هذا الاستدعاء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| msLimit | int | الحد الزمني (مللي ثانية) المطلوب للمقاطعة. |

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

