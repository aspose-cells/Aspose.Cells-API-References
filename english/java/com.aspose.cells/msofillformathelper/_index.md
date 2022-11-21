---
title: MsoFillFormatHelper
second_title: Aspose.Cells for Java API Reference
description: Represents fill formatting for a shape.
type: docs
weight: 330
url: /java/com.aspose.cells/msofillformathelper/
---

**Inheritance:**
java.lang.Object
```
public class MsoFillFormatHelper
```

Represents fill formatting for a shape.
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | the file back color. |
| [getClass()](#getClass--) |  |
| [getForeColor()](#getForeColor--) | the fill fore color. |
| [getForeColorTransparency()](#getForeColorTransparency--) | Returns or sets the degree of fore color of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
| [getImageData()](#getImageData--) | the Texture and Picture fill data. |
| [getTexture()](#getTexture--) | Gets the texture fill type. |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | Indicates whether there is fill. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.cells.Color-) | For the description of this property, please see [getBackColor()](../../com.aspose.cells/msofillformathelper\#getBackColor--) |
| [setForeColor(Color value)](#setForeColor-com.aspose.cells.Color-) | For the description of this property, please see [getForeColor()](../../com.aspose.cells/msofillformathelper\#getForeColor--) |
| [setForeColorTransparency(double value)](#setForeColorTransparency-double-) | For the description of this property, please see [getForeColorTransparency()](../../com.aspose.cells/msofillformathelper\#getForeColorTransparency--) |
| [setImageData(byte[] value)](#setImageData-byte---) | For the description of this property, please see [getImageData()](../../com.aspose.cells/msofillformathelper\#getImageData--) |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Sets the specified fill to a one-color gradient. |
| [setVisible(boolean value)](#setVisible-boolean-) | For the description of this property, please see [isVisible()](../../com.aspose.cells/msofillformathelper\#isVisible--) |
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
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


the file back color.

**Returns:**
[Color](../../com.aspose.cells/color)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


the fill fore color.

**Returns:**
[Color](../../com.aspose.cells/color)
### getForeColorTransparency() {#getForeColorTransparency--}
```
public double getForeColorTransparency()
```


Returns or sets the degree of fore color of the specified fill as a value from 0.0 (opaque) through 1.0 (clear).

**Returns:**
double
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


the Texture and Picture fill data.

**Returns:**
byte[]
### getTexture() {#getTexture--}
```
public int getTexture()
```


Gets the texture fill type.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Indicates whether there is fill.

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




### setBackColor(Color value) {#setBackColor-com.aspose.cells.Color-}
```
public void setBackColor(Color value)
```


For the description of this property, please see [getBackColor()](../../com.aspose.cells/msofillformathelper\#getBackColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColor(Color value) {#setForeColor-com.aspose.cells.Color-}
```
public void setForeColor(Color value)
```


For the description of this property, please see [getForeColor()](../../com.aspose.cells/msofillformathelper\#getForeColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColorTransparency(double value) {#setForeColorTransparency-double-}
```
public void setForeColorTransparency(double value)
```


For the description of this property, please see [getForeColorTransparency()](../../com.aspose.cells/msofillformathelper\#getForeColorTransparency--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


For the description of this property, please see [getImageData()](../../com.aspose.cells/msofillformathelper\#getImageData--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Sets the specified fill to a one-color gradient.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | One gradient color. |
| degree | double | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | int | Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


For the description of this property, please see [isVisible()](../../com.aspose.cells/msofillformathelper\#isVisible--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

