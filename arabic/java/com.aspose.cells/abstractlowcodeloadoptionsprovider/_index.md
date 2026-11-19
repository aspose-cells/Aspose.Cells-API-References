---
title: "AbstractLowCodeLoadOptionsProvider"
second_title: "Aspose.Cells for Java API Reference"
description: "تنفيذ لتوفير خيارات تحميل متعددة للعمليات التي تستخدم مدخلات متعددة مثل ملفات القالب."
type: docs
url: /ar/java/com.aspose.cells/abstractlowcodeloadoptionsprovider/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractLowCodeLoadOptionsProvider
```

تنفيذ لتوفير خيارات تحميل متعددة للعمليات التي تستخدم مدخلات متعددة (مثل ملفات القالب).

**Remarks**

على سبيل المثال، الميزة [SpreadsheetMerger](../../com.aspose.cells/spreadsheetmerger) تتطلب ملفات قالب متعددة للدمج.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [AbstractLowCodeLoadOptionsProvider()](#AbstractLowCodeLoadOptionsProvider--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeLoadOptions part)](#finish-com.aspose.cells.LowCodeLoadOptions-) | يطلق الموارد بعد معالجة الجزء الحالي من المدخلات. |
| [getClass()](#getClass--) |  |
| [getCurrent()](#getCurrent--) | يحصل على خيارات التحميل التي يتم منها تحميل بيانات الجزء المعالج حاليًا. |
| [hashCode()](#hashCode--) |  |
| [moveNext()](#moveNext--) | يتحقق مما إذا كان هناك المزيد من المدخلات. |
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### finish(LowCodeLoadOptions part) {#finish-com.aspose.cells.LowCodeLoadOptions-}
```
public void finish(LowCodeLoadOptions part)
```


يطلق الموارد بعد معالجة الجزء الحالي من المدخلات.

**Remarks**

بشكل افتراضي، تقوم هذه الطريقة فقط بإغلاق الدفق المحدد بواسطة [LowCodeLoadOptions.getInputStream()](../../com.aspose.cells/lowcodeloadoptions\#getInputStream--) مباشرةً (إذا حددت خيارات التحميل دفقًا كمصدر). يمكن للمستخدم استبدال هذه الطريقة للتحكم في كيفية تحرير الموارد وفقًا لمتطلباته وتنفيذ [getCurrent()](../../com.aspose.cells/abstractlowcodeloadoptionsprovider\#getCurrent--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| part | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | خيارات التحميل المستخدمة للجزء المقسّم حاليًا. |

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


يحصل على خيارات التحميل التي يتم منها تحميل بيانات الجزء المعالج حاليًا.

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


يتحقق مما إذا كان هناك المزيد من المدخلات.

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

