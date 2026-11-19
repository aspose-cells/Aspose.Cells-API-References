---
title: "MsoFillFormatHelper"
second_title: "Aspose.Cells for Java API 参考"
description: "表示形状的填充格式。"
type: docs
url: /zh/java/com.aspose.cells/msofillformathelper/
---

**Inheritance:**
java.lang.Object
```
public class MsoFillFormatHelper
```

表示形状的填充格式。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | 获取文件的背景颜色。 |
| [getClass()](#getClass--) |  |
| [getForeColor()](#getForeColor--) | 获取填充的前景颜色。 |
| [getForeColorTransparency()](#getForeColorTransparency--) | 返回或设置指定填充的前景颜色程度，取值范围为 0.0（不透明）至 1.0（透明）。 |
| [getImageData()](#getImageData--) | 获取纹理和图片填充数据。 |
| [getTexture()](#getTexture--) | 获取纹理填充类型。 |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | 指示是否存在填充。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.cells.Color-) | 设置文件的背景颜色。 |
| [setForeColor(Color value)](#setForeColor-com.aspose.cells.Color-) | 设置填充的前景颜色。 |
| [setForeColorTransparency(double value)](#setForeColorTransparency-double-) | 返回或设置指定填充的前景颜色程度，取值范围为 0.0（不透明）至 1.0（透明）。 |
| [setImageData(byte[] value)](#setImageData-byte---) | 设置纹理和图片填充数据。 |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | 将指定填充设置为单色渐变。 |
| [setVisible(boolean value)](#setVisible-boolean-) | 指示是否存在填充。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


获取文件的背景颜色。

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


获取填充的前景颜色。

**Returns:**
[Color](../../com.aspose.cells/color)
### getForeColorTransparency() {#getForeColorTransparency--}
```
public double getForeColorTransparency()
```


返回或设置指定填充的前景颜色程度，取值范围为 0.0（不透明）至 1.0（透明）。

**Returns:**
double
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


获取纹理和图片填充数据。

**Returns:**
byte[]
### getTexture() {#getTexture--}
```
public int getTexture()
```


获取纹理填充类型。

参见 [TextureType](../../com.aspose.cells/texturetype)。

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


指示是否存在填充。

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


设置文件的背景颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColor(Color value) {#setForeColor-com.aspose.cells.Color-}
```
public void setForeColor(Color value)
```


设置填充的前景颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColorTransparency(double value) {#setForeColorTransparency-double-}
```
public void setForeColorTransparency(double value)
```


返回或设置指定填充的前景颜色程度，取值范围为 0.0（不透明）至 1.0（透明）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


设置纹理和图片填充数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte[] |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


将指定填充设置为单色渐变。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | 单一渐变颜色。 |
| degree | double | 渐变的度数。取值范围为 0.0（暗）至 1.0（亮）。 |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype)。渐变阴影样式。 |
| variant | int | 渐变的变体。取值范围为 1 到 4，对应“填充效果”对话框中“渐变”选项卡上的四种变体之一。如果样式为 GradientStyle.FromCenter，则 Variant 参数只能为 1 或 2。 |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


指示是否存在填充。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

