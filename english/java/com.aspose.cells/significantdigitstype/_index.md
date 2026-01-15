---
title: SignificantDigitsType
second_title: Aspose.Cells for Java API Reference
description: Represents the type of significant digits for outputting numeric values.
type: docs
url: /java/com.aspose.cells/significantdigitstype/
---

**Inheritance:**
java.lang.Object
```
public final class SignificantDigitsType
```

Represents the type of significant digits for outputting numeric values.
## Fields

| Field | Description |
| --- | --- |
| [DIGITS_15](#DIGITS-15) | 15-digits |
| [G_17](#G-17) | 17-digits by formatting the value with "G17". |
| [ROUNDING_17](#ROUNDING-17) | 17-digits by rounding the value. |
## Methods

| Method | Description |
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
### DIGITS_15 {#DIGITS-15}
```
public static final int DIGITS_15
```


15-digits

### G_17 {#G-17}
```
public static final int G_17
```


17-digits by formatting the value with "G17".

**Remarks**

For some double values, "G17" may given different value than the original/literal one input by user. For example, double value 0.15 will be output as 0.14999999999999999; double value 1.0E-16 will be output as 9.9999999999999998E-17. Ms excel's handles those values inconsistently, it saves 0.15 as 0.15 in the xlsx file, but for 1.0E-16 the saved value in the xlsx file is 9.9999999999999998E-17.

### ROUNDING_17 {#ROUNDING-17}
```
public static final int ROUNDING_17
```


17-digits by rounding the value.

**Remarks**

This type generally outputs the value as the original/literal one input by user. For 0.15 it produces "0.15" and for 1.0E-16 it produces "1.0E-16". But there are also some special cases which may give different values than the literal. For example, when rounding 208435494.96478021 to 17-digits("0.\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#"), the output is 208435494.96478.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

