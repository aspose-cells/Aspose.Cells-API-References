---
title: "CellValueFormatStrategy"
second_title: "Aspose.Cells for Java API Reference"
description: "يحدد كيفية تطبيق النمط لقيمة الخلية."
type: docs
url: /ar/java/com.aspose.cells/cellvalueformatstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CellValueFormatStrategy
```

يحدد كيفية تطبيق النمط لقيمة الخلية.
## حقول

| حقل | الوصف |
| --- | --- |
| [CELL_STYLE](#CELL-STYLE) | مُنسق فقط باستخدام النمط الأصلي للخلية. |
| [DISPLAY_STRING](#DISPLAY-STRING) | يحصل على السلسلة المعروضة في MS Excel. |
| [DISPLAY_STYLE](#DISPLAY-STYLE) | مُنسق باستخدام النمط المعروض للخلية. |
| [NONE](#NONE) | غير مُنسق. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CELL_STYLE {#CELL-STYLE}
```
public static final int CELL_STYLE
```


مُنسق فقط باستخدام النمط الأصلي للخلية.

### DISPLAY_STRING {#DISPLAY-STRING}
```
public static final int DISPLAY_STRING
```


يحصل على السلسلة المعروضة في MS Excel. الاختلاف الرئيسي عن [DISPLAY\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#DISPLAY-STYLE) هو أن هذا الخيار يأخذ في الاعتبار تأثير عرض العمود أيضًا. إذا كان عرض العمود صغيرًا جدًا لعرض السلسلة المُنسقة بالكامل، قد يتم عرض "\\#"، كما يحدث في MS Excel.

### DISPLAY_STYLE {#DISPLAY-STYLE}
```
public static final int DISPLAY_STYLE
```


مُنسق باستخدام النمط المعروض للخلية.

### NONE {#NONE}
```
public static final int NONE
```


غير مُنسق.

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

