---
title: "SetBorderPosition"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل موضع الحدود الذي سيتم تعيينه لنطاق الخلايا."
type: docs
url: /ar/java/com.aspose.gridweb/setborderposition/
---

**Inheritance:**
java.lang.Object
```
public final class SetBorderPosition
```

يمثل موضع الحدود الذي سيتم تعيينه لنطاق الخلايا.

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, GridWeb1.getWorkSheets().get(0).getCells().get(0, 0).getStyle().getLeftBorderStyle());
```
## حقول

| حقل | الوصف |
| --- | --- |
| [BOTTOM](#BOTTOM) | الحد السفلي |
| [CROSS](#CROSS) | حدود متقاطعة |
| [HORIZONTAL_MIDDLE](#HORIZONTAL-MIDDLE) | الحد السفلي |
| [LEFT](#LEFT) | الحد الأيسر |
| [NONE](#NONE) | بدون حدود |
| [OUTLINE](#OUTLINE) | حدود العمودي المتوسط |
| [RIGHT](#RIGHT) | الحد الأيمن |
| [TOP](#TOP) | الحد العلوي |
| [VERTICAL_MIDDLE](#VERTICAL-MIDDLE) | حدود الأفقية المتوسطة |
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
### BOTTOM {#BOTTOM}
```
public static final int BOTTOM
```


الحد السفلي

### CROSS {#CROSS}
```
public static final int CROSS
```


حدود متقاطعة

### HORIZONTAL_MIDDLE {#HORIZONTAL-MIDDLE}
```
public static final int HORIZONTAL_MIDDLE
```


الحد السفلي

### LEFT {#LEFT}
```
public static final int LEFT
```


الحد الأيسر

### NONE {#NONE}
```
public static final int NONE
```


بدون حدود

### OUTLINE {#OUTLINE}
```
public static final int OUTLINE
```


حدود العمودي المتوسط

### RIGHT {#RIGHT}
```
public static final int RIGHT
```


الحد الأيمن

### TOP {#TOP}
```
public static final int TOP
```


الحد العلوي

### VERTICAL_MIDDLE {#VERTICAL-MIDDLE}
```
public static final int VERTICAL_MIDDLE
```


حدود الأفقية المتوسطة

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

