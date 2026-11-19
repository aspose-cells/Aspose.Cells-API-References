---
title: "LowCodeHtmlSaveOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "خيارات حفظ HTML بطريقة منخفضة الكود."
type: docs
url: /ar/java/com.aspose.cells/lowcodehtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeHtmlSaveOptions extends LowCodeSaveOptions
```

خيارات حفظ HTML بطريقة منخفضة الكود.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [LowCodeHtmlSaveOptions()](#LowCodeHtmlSaveOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHtmlOptions()](#getHtmlOptions--) | الخيارات العامة لحفظ HTML. |
| [getOutputFile()](#getOutputFile--) | يحصل على الملف (مع المسار إذا لزم) لحفظ البيانات المولدة. |
| [getOutputStream()](#getOutputStream--) | يحصل على الدفق لكتابة البيانات المولدة إليه. |
| [getSaveFormat()](#getSaveFormat--) | يحصل على تنسيق جدول البيانات. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHtmlOptions(HtmlSaveOptions value)](#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-) | الخيارات العامة لحفظ HTML. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | يضبط الملف (مع المسار إذا لزم) لحفظ البيانات المولدة. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | يضبط الدفق لكتابة البيانات المولدة إليه. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | يضبط تنسيق جدول البيانات. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeHtmlSaveOptions() {#LowCodeHtmlSaveOptions--}
```
public LowCodeHtmlSaveOptions()
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
### getHtmlOptions() {#getHtmlOptions--}
```
public HtmlSaveOptions getHtmlOptions()
```


الخيارات العامة لحفظ HTML.

**Remarks**

عند تحديد نسخة واحدة من [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)، سيتم استبدال [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) (إذا تم تحديده مسبقًا).

**Returns:**
[HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)
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


يحصل على تنسيق جدول البيانات.

انظر [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

عند تغيير هذه الخاصية، سيتم تجاهل تنسيق الحفظ المحدد بواسطة [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) (إذا تم تحديده مسبقًا).

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




### setHtmlOptions(HtmlSaveOptions value) {#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-}
```
public void setHtmlOptions(HtmlSaveOptions value)
```


الخيارات العامة لحفظ HTML.

**Remarks**

عند تحديد نسخة واحدة من [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)، سيتم استبدال [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) (إذا تم تحديده مسبقًا).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) |  |

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


يضبط تنسيق جدول البيانات.

انظر [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

عند تغيير هذه الخاصية، سيتم تجاهل تنسيق الحفظ المحدد بواسطة [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) (إذا تم تحديده مسبقًا).

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

