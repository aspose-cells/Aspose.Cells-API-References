---
title: "StreamProviderOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خيارات الدفق."
type: docs
url: /ar/java/com.aspose.cells/streamprovideroptions/
---

**Inheritance:**
java.lang.Object
```
public class StreamProviderOptions
```

يمثل خيارات الدفق.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [StreamProviderOptions(int loadingType, String defaultPath)](#StreamProviderOptions-int-java.lang.String-) | ينشئ مثيلاً جديدًا من الفئة [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions). |
| [StreamProviderOptions()](#StreamProviderOptions--) | ينشئ مثيلاً جديدًا من الفئة [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomPath()](#getCustomPath--) | المسار المخصص للمستخدم (URL) المحفوظ في ملف HTML المُولد للمصدر المشار إليه. |
| [getDefaultPath()](#getDefaultPath--) | المسار الافتراضي (URL) المحفوظ في ملف HTML المُولد للمصدر المشار إليه. |
| [getInputStream()](#getInputStream--) | يحصل على تدفق الإدخال للحصول على البيانات. |
| [getResourceLoadingType()](#getResourceLoadingType--) | يحصل على نوع مورد التحميل. |
| [getStream()](#getStream--) | يحصل على تدفق الإخراج لكتابة البيانات المحفوظة. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomPath(String value)](#setCustomPath-java.lang.String-) | المسار المخصص للمستخدم (URL) المحفوظ في ملف HTML المُولد للمصدر المشار إليه. |
| [setInputStream(InputStream value)](#setInputStream-java.io.InputStream-) | يضبط تدفق الإدخال للحصول على البيانات. |
| [setResourceLoadingType(int value)](#setResourceLoadingType-int-) | يضبط نوع مورد التحميل. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | يضبط تدفق الإخراج لكتابة البيانات المحفوظة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### StreamProviderOptions(int loadingType, String defaultPath) {#StreamProviderOptions-int-java.lang.String-}
```
public StreamProviderOptions(int loadingType, String defaultPath)
```


ينشئ مثيلاً جديدًا من الفئة [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| loadingType | int | [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype). النوع لتحميل المورد المرتبط. |
| defaultPath | java.lang.String | المسار الافتراضي. |

### StreamProviderOptions() {#StreamProviderOptions--}
```
public StreamProviderOptions()
```


ينشئ مثيلاً جديدًا من الفئة [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions).

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
### getCustomPath() {#getCustomPath--}
```
public String getCustomPath()
```


المسار المخصص للمستخدم (URL) المحفوظ في ملف HTML المُولد للمصدر المشار إليه. إذا لم يحدده المستخدم، سيُستخدم DefaultPath. على سبيل المثال، سيحفظ المستخدم بيانات الورقة إلى d:/sheet001.htm، ويجب أن يكون عنوان URL المستخدم في ملف HTML الرئيسي هو \"d:/sheet001.htm\" أو أي مسار نسبي صالح يمكن الوصول إليه من ملف HTML الرئيسي.

**Returns:**
java.lang.String
### getDefaultPath() {#getDefaultPath--}
```
public String getDefaultPath()
```


المسار الافتراضي (URL) المحفوظ في ملف HTML المُولد للمصدر المشار إليه. على سبيل المثال، تُحفظ بيانات الورقة في xxx\\_files/sheet001.htm، ويجب أن يكون عنوان URL المستخدم في ملف HTML الرئيسي مثل \"src=\"xxx\\_files/sheet001.htm\"\".

**Returns:**
java.lang.String
### getInputStream() {#getInputStream--}
```
public InputStream getInputStream()
```


يحصل على تدفق الإدخال للحصول على البيانات.

**Returns:**
java.io.InputStream
### getResourceLoadingType() {#getResourceLoadingType--}
```
public int getResourceLoadingType()
```


يحصل على نوع مورد التحميل.

انظر [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Returns:**
int
### getStream() {#getStream--}
```
public OutputStream getStream()
```


يحصل على تدفق الإخراج لكتابة البيانات المحفوظة.

**Returns:**
java.io.OutputStream
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




### setCustomPath(String value) {#setCustomPath-java.lang.String-}
```
public void setCustomPath(String value)
```


المسار المخصص للمستخدم (URL) المحفوظ في ملف HTML المُولد للمصدر المشار إليه. إذا لم يحدده المستخدم، سيُستخدم DefaultPath. على سبيل المثال، سيحفظ المستخدم بيانات الورقة إلى d:/sheet001.htm، ويجب أن يكون عنوان URL المستخدم في ملف HTML الرئيسي هو \"d:/sheet001.htm\" أو أي مسار نسبي صالح يمكن الوصول إليه من ملف HTML الرئيسي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setInputStream(InputStream value) {#setInputStream-java.io.InputStream-}
```
public void setInputStream(InputStream value)
```


يضبط تدفق الإدخال للحصول على البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.io.InputStream |  |

### setResourceLoadingType(int value) {#setResourceLoadingType-int-}
```
public void setResourceLoadingType(int value)
```


يضبط نوع مورد التحميل.

انظر [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public void setStream(OutputStream value)
```


يضبط تدفق الإخراج لكتابة البيانات المحفوظة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.io.OutputStream |  |

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

