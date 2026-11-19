---
title: "LowCodeSaveOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "خيارات حفظ النتائج المولدة بطريقة منخفضة الكود."
type: docs
url: /ar/java/com.aspose.cells/lowcodesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class LowCodeSaveOptions
```

خيارات حفظ النتائج المولدة بطريقة منخفضة الكود.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [LowCodeSaveOptions()](#LowCodeSaveOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOutputFile()](#getOutputFile--) | يحصل على الملف (مع المسار إذا لزم) لحفظ البيانات المولدة. |
| [getOutputStream()](#getOutputStream--) | يحصل على الدفق لكتابة البيانات المولدة إليه. |
| [getSaveFormat()](#getSaveFormat--) | يحصل على تنسيق الحفظ للإخراج. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | يضبط الملف (مع المسار إذا لزم) لحفظ البيانات المولدة. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | يضبط الدفق لكتابة البيانات المولدة إليه. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | يضبط تنسيق الحفظ للإخراج. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptions() {#LowCodeSaveOptions--}
```
public LowCodeSaveOptions()
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
### getOutputFile() {#getOutputFile--}
```
public String getOutputFile()
```


يحصل على الملف (مع المسار إذا لزم) لحفظ البيانات المولدة. عند ضبط هذه الخاصية بقيمة غير null أو سلسلة فارغة، سيتم تجاهل [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--).

**Returns:**
java.lang.String
### getOutputStream() {#getOutputStream--}
```
public InputStream getOutputStream()
```


يحصل على الدفق لكتابة البيانات المولدة إليه. عند ضبط هذه الخاصية بقيمة غير null، سيتم تجاهل [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--).

**Returns:**
java.io.InputStream
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


يحصل على تنسيق الحفظ للإخراج. بشكل عام، بالنسبة للعمليات المحددة بطريقة منخفضة الشيفرة، يُسمح فقط ببعض التنسيقات المحددة. يرجى تحديد التنسيق الصحيح للعملية المقابلة، وإلا قد يحدث نتيجة غير متوقعة أو حتى استثناء.

انظر [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
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




### setOutputFile(String value) {#setOutputFile-java.lang.String-}
```
public void setOutputFile(String value)
```


يضبط الملف (مع المسار إذا لزم) لحفظ البيانات المولدة. عند ضبط هذه الخاصية بقيمة غير null أو سلسلة فارغة، سيتم تجاهل [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOutputStream(InputStream value) {#setOutputStream-java.io.InputStream-}
```
public void setOutputStream(InputStream value)
```


يضبط الدفق لكتابة البيانات المولدة إليه. عند ضبط هذه الخاصية بقيمة غير null، سيتم تجاهل [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.io.InputStream |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


يضبط تنسيق الحفظ للإخراج. بشكل عام، بالنسبة للعمليات المحددة بطريقة منخفضة الشيفرة، يُسمح فقط ببعض التنسيقات المحددة. يرجى تحديد التنسيق الصحيح للعملية المقابلة، وإلا قد يحدث نتيجة غير متوقعة أو حتى استثناء.

انظر [SaveFormat](../../com.aspose.cells/saveformat).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

