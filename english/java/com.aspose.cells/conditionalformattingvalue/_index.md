---
title: ConditionalFormattingValue
second_title: Aspose.Cells for Java API Reference
description: Describes the values of the interpolation points in a gradient scale dataBar or iconSet.
type: docs
weight: 110
url: /java/com.aspose.cells/conditionalformattingvalue/
---

**Inheritance:**
java.lang.Object
```
public class ConditionalFormattingValue
```

Describes the values of the interpolation points in a gradient scale, dataBar or iconSet.
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | the type of this conditional formatting value object. |
| [getValue()](#getValue--) | the value of this conditional formatting value object. |
| [hashCode()](#hashCode--) |  |
| [isGTE()](#isGTE--) | the Greater Than Or Equal flag. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setGTE(boolean value)](#setGTE-boolean-) | For the description of this property, please see [isGTE()](../../com.aspose.cells/conditionalformattingvalue\#isGTE--) |
| [setType(int value)](#setType-int-) | For the description of this property, please see [getType()](../../com.aspose.cells/conditionalformattingvalue\#getType--) |
| [setValue(Object value)](#setValue-java.lang.Object-) | For the description of this property, please see [getValue()](../../com.aspose.cells/conditionalformattingvalue\#getValue--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getType() {#getType--}
```
public int getType()
```


the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null.

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


the value of this conditional formatting value object. It should be used in conjunction with Type. If the value is string and start with "=", it will be processed as a formula, otherwise we will process it as a simple value.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGTE() {#isGTE--}
```
public boolean isGTE()
```


the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true.

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




### setGTE(boolean value) {#setGTE-boolean-}
```
public void setGTE(boolean value)
```


For the description of this property, please see [isGTE()](../../com.aspose.cells/conditionalformattingvalue\#isGTE--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


For the description of this property, please see [getType()](../../com.aspose.cells/conditionalformattingvalue\#getType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


For the description of this property, please see [getValue()](../../com.aspose.cells/conditionalformattingvalue\#getValue--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |

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

