---
title: "Encoding"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل ترميزًا أحرفيًا."
type: docs
url: /ar/java/com.aspose.gridweb/encoding/
---

**Inheritance:**
java.lang.Object
```
public class Encoding
```

يمثل ترميزًا أحرفيًا.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Encoding()](#Encoding--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Encoding other)](#equals-com.aspose.gridweb.Encoding-) | يحدد ما إذا كان كائن Encoding المحدد يساوي المثيل الحالي. |
| [equals(Object o)](#equals-java.lang.Object-) | يحدد ما إذا كان الكائن المحدد يساوي المثيل الحالي. |
| [getASCII()](#getASCII--) | يحصل على ترميز لمجموعة الأحرف ASCII (7 بت). |
| [getBigEndianUnicode()](#getBigEndianUnicode--) | يحصل على ترميز لتنسيق UTF-16 باستخدام ترتيب البايتات كبير النهاية. |
| [getClass()](#getClass--) |  |
| [getDefault()](#getDefault--) | يحصل على ترميز لصفحة الشيفرة ANSI الحالية لنظام التشغيل. |
| [getEncoding(int codePage)](#getEncoding-int-) | يعيد الترميز المرتبط بمعرّف صفحة الشيفرة المحدد. |
| [getEncoding(String charsetName)](#getEncoding-java.lang.String-) | يعيد ترميزًا مرتبطًا باسم مجموعة الأحرف المحدد. |
| [getEncoding(Charset charset)](#getEncoding-java.nio.charset.Charset-) | إرجاع ترميز مرتبط بكائن مجموعة الأحرف المحدد. |
| [getUTF7()](#getUTF7--) | الحصول على ترميز لتنسيق UTF-7. |
| [getUTF8()](#getUTF8--) | الحصول على ترميز لتنسيق UTF-8. |
| [getUTF8NoBOM()](#getUTF8NoBOM--) | الحصول على ترميز لتنسيق UTF-8 بدون معرف UTF-8. |
| [getUnicode()](#getUnicode--) | الحصول على ترميز لتنسيق UTF-16 باستخدام ترتيب البايت الصغير (little endian). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Encoding() {#Encoding--}
```
public Encoding()
```


### equals(Encoding other) {#equals-com.aspose.gridweb.Encoding-}
```
public boolean equals(Encoding other)
```


يحدد ما إذا كان كائن Encoding المحدد يساوي المثيل الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [Encoding](../../com.aspose.gridweb/encoding) | كائن Encoding للمقارنة مع المثيل الحالي. |

**Returns:**
boolean - true إذا كانت القيمة مساوية للمثيل الحالي؛ وإلا false.
### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


يحدد ما إذا كان الكائن المحدد يساوي المثيل الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | الكائن للمقارنة مع المثيل الحالي. |

**Returns:**
boolean - true إذا كانت القيمة مثيلًا لـ Encoding ومساوية للمثيل الحالي؛ وإلا false.
### getASCII() {#getASCII--}
```
public static Encoding getASCII()
```


يحصل على ترميز لمجموعة الأحرف ASCII (7 بت).

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the ASCII (7-bit) character set.
### getBigEndianUnicode() {#getBigEndianUnicode--}
```
public static Encoding getBigEndianUnicode()
```


يحصل على ترميز لتنسيق UTF-16 باستخدام ترتيب البايتات كبير النهاية.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-16 format using the big endian byte
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefault() {#getDefault--}
```
public static Encoding getDefault()
```


يحصل على ترميز لصفحة الشيفرة ANSI الحالية لنظام التشغيل.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - An encoding for the operating system's current ANSI code page.
### getEncoding(int codePage) {#getEncoding-int-}
```
public static Encoding getEncoding(int codePage)
```


يعيد الترميز المرتبط بمعرّف صفحة الشيفرة المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| codePage | int | معرف صفحة الترميز للترميز المفضل. -or- 0 لاستخدام الترميز الافتراضي. |

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified code page.
### getEncoding(String charsetName) {#getEncoding-java.lang.String-}
```
public static Encoding getEncoding(String charsetName)
```


يعيد ترميزًا مرتبطًا باسم مجموعة الأحرف المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| charsetName | java.lang.String | اسم مجموعة الأحرف المحدد |

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified charset name.
### getEncoding(Charset charset) {#getEncoding-java.nio.charset.Charset-}
```
public static Encoding getEncoding(Charset charset)
```


إرجاع ترميز مرتبط بكائن مجموعة الأحرف المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| charset | java.nio.charset.Charset | كائن مجموعة الأحرف المحدد |

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified charset object.
### getUTF7() {#getUTF7--}
```
public static Encoding getUTF7()
```


الحصول على ترميز لتنسيق UTF-7.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-7 format.
### getUTF8() {#getUTF8--}
```
public static Encoding getUTF8()
```


الحصول على ترميز لتنسيق UTF-8.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-8 format.
### getUTF8NoBOM() {#getUTF8NoBOM--}
```
public static Encoding getUTF8NoBOM()
```


الحصول على ترميز لتنسيق UTF-8 بدون معرف UTF-8.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-8 format without UTF-8 identifier.
### getUnicode() {#getUnicode--}
```
public static Encoding getUnicode()
```


الحصول على ترميز لتنسيق UTF-16 باستخدام ترتيب البايت الصغير (little endian).

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-16 format using the little endian byte
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

