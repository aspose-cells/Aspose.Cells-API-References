---
title: "DefaultStyleSettings"
second_title: "Aspose.Cells for Java API Reference"
description: "إعدادات القيم الافتراضية لخصائص نمط المصنفات."
type: docs
url: /ar/java/com.aspose.cells/defaultstylesettings/
---

**Inheritance:**
java.lang.Object
```
public class DefaultStyleSettings
```

إعدادات القيم الافتراضية لخصائص نمط المصنف.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuiltInPreference()](#getBuiltInPreference--) | يشير إلى ما إذا كانت الخاصية لتنسيق الأرقام مفضلة عندما يحدد النمط كلًا من الرقم المدمج والنمط المخصص. |
| [getClass()](#getClass--) |  |
| [getFontName()](#getFontName--) | يحصل على اسم الخط الافتراضي للمصنف |
| [getFontSize()](#getFontSize--) | يحصل على حجم الخط القياسي الافتراضي للمصنف. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | يحصل على القيمة الافتراضية للمحاذاة الأفقية |
| [getVerticalAlignment()](#getVerticalAlignment--) | يحصل على القيمة الافتراضية للمحاذاة العمودية |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuiltInPreference(boolean value)](#setBuiltInPreference-boolean-) | يشير إلى ما إذا كانت الخاصية لتنسيق الأرقام مفضلة عندما يحدد النمط كلًا من الرقم المدمج والنمط المخصص. |
| [setFontName(String value)](#setFontName-java.lang.String-) | يضبط اسم الخط الافتراضي لدفتر العمل |
| [setFontSize(double value)](#setFontSize-double-) | يضبط حجم الخط القياسي الافتراضي لدفتر العمل. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | يضبط القيمة الافتراضية للمحاذاة الأفقية |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | يضبط القيمة الافتراضية للمحاذاة العمودية |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getBuiltInPreference() {#getBuiltInPreference--}
```
public boolean getBuiltInPreference()
```


يشير إلى ما إذا كانت الخاصية لتنسيق الأرقام مفضلة عندما يحدد النمط كلًا من الرقم المدمج والنمط المخصص. القيمة الافتراضية هي false، وهذا يعني أنه بشكل افتراضي سيُستخدم النمط المخصص لتنسيق القيم طالما أنه غير فارغ لنمط واحد.

**Remarks**

عند تحميل دفتر العمل من ملف قالب موجود، قد يتم تعريف كل من الرقم المدمج والنمط المخصص لنمط واحد. تحدد هذه الخاصية ما إذا كنا يجب أن نستخدم الرقم المدمج أو النمط المخصص عند تنسيق القيم باستخدام النمط.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFontName() {#getFontName--}
```
public String getFontName()
```


يحصل على اسم الخط الافتراضي للمصنف

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


يحصل على حجم الخط القياسي الافتراضي للمصنف.

**Returns:**
double
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


يحصل على القيمة الافتراضية للمحاذاة الأفقية

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


يحصل على القيمة الافتراضية للمحاذاة العمودية

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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




### setBuiltInPreference(boolean value) {#setBuiltInPreference-boolean-}
```
public void setBuiltInPreference(boolean value)
```


يشير إلى ما إذا كانت الخاصية لتنسيق الأرقام مفضلة عندما يحدد النمط كلًا من الرقم المدمج والنمط المخصص. القيمة الافتراضية هي false، وهذا يعني أنه بشكل افتراضي سيُستخدم النمط المخصص لتنسيق القيم طالما أنه غير فارغ لنمط واحد.

**Remarks**

عند تحميل دفتر العمل من ملف قالب موجود، قد يتم تعريف كل من الرقم المدمج والنمط المخصص لنمط واحد. تحدد هذه الخاصية ما إذا كنا يجب أن نستخدم الرقم المدمج أو النمط المخصص عند تنسيق القيم باستخدام النمط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


يضبط اسم الخط الافتراضي لدفتر العمل

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setFontSize(double value) {#setFontSize-double-}
```
public void setFontSize(double value)
```


يضبط حجم الخط القياسي الافتراضي لدفتر العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


يضبط القيمة الافتراضية للمحاذاة الأفقية

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


يضبط القيمة الافتراضية للمحاذاة العمودية

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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

