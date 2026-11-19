---
title: "GradientFill"
second_title: "Aspose.Cells for Java API 参考"
description: "表示渐变填充。"
type: docs
url: /zh/java/com.aspose.cells/gradientfill/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Fill](../../com.aspose.cells/fill)
```
public class GradientFill extends Fill
```

表示渐变填充。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | / |
| [getAngle()](#getAngle--) | 线性填充的角度。 |
| [getClass()](#getClass--) |  |
| [getDirectionType()](#getDirectionType--) | 获取渐变方向类型。 |
| [getFillType()](#getFillType--) | 获取渐变填充类型。 |
| [getGradientColor1()](#getGradientColor1--) | 获取渐变颜色 1。 |
| [getGradientColor2()](#getGradientColor2--) | 获取渐变颜色 2。 |
| [getGradientColorType()](#getGradientColorType--) | 获取渐变颜色类型。 |
| [getGradientDegree()](#getGradientDegree--) | 获取渐变角度。 |
| [getGradientStops()](#getGradientStops--) | 表示渐变停止点集合。 |
| [getGradientStyle()](#getGradientStyle--) | 获取渐变样式类型。 |
| [getPresetColor()](#getPresetColor--) | 返回指定填充的渐变预设颜色。 |
| [getVariant()](#getVariant--) | 获取变体。 |
| [hashCode()](#hashCode--) | 获取哈希码。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAngle(float value)](#setAngle-float-) | 线性填充的角度。 |
| [setGradient(int type, double angle, int direction)](#setGradient-int-double-int-) | 设置渐变填充类型和方向。 |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | 将指定填充设置为单色渐变。 |
| [setPresetColor(int value)](#setPresetColor-int-) | 返回指定填充的渐变预设颜色。 |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | 将指定填充设置为预设颜色渐变。 |
| [setPresetThemeGradient(int gradientType, int themeColorType)](#setPresetThemeGradient-int-int-) | 设置预设主题渐变填充。 |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | 将指定填充设置为双色渐变。 |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | 将指定填充设置为双色渐变。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


/

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getAngle() {#getAngle--}
```
public float getAngle()
```


线性填充的角度。

**Returns:**
float
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


获取渐变方向类型。

参见 [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype)。

**Returns:**
int
### getFillType() {#getFillType--}
```
public int getFillType()
```


获取渐变填充类型。

参见 [GradientFillType](../../com.aspose.cells/gradientfilltype)。

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


获取渐变颜色 1。适用于 Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


获取渐变颜色 2。适用于 Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


获取渐变颜色类型。适用于 Excel97-2003

参见 [GradientColorType](../../com.aspose.cells/gradientcolortype)。

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


获取渐变角度。适用于 Excel97-2003

**Returns:**
double
### getGradientStops() {#getGradientStops--}
```
public GradientStopCollection getGradientStops()
```


表示渐变停止点集合。

**Returns:**
[GradientStopCollection](../../com.aspose.cells/gradientstopcollection)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


获取渐变样式类型。适用于 Excel97-2003

参见 [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


返回指定填充的渐变预设颜色。适用于 Excel97-2003

参见 [GradientPresetType](../../com.aspose.cells/gradientpresettype)。

**Returns:**
int
### getVariant() {#getVariant--}
```
public int getVariant()
```


获取变体。适用于 Excel97-2003

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


获取哈希码。

**Returns:**
int -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAngle(float value) {#setAngle-float-}
```
public void setAngle(float value)
```


线性填充的角度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setGradient(int type, double angle, int direction) {#setGradient-int-double-int-}
```
public void setGradient(int type, double angle, int direction)
```


设置渐变填充类型和方向。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [GradientFillType](../../com.aspose.cells/gradientfilltype)。渐变填充类型。 |
| 角度 | double | 角度。仅适用于 GradientFillType.Linear。 |
| direction | int | [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype)。方向类型。仅适用于 GradientFillType.Radial 和 GradientFillType.Rectangle。 |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


将指定的填充设置为单色渐变。仅适用于 Excel 2007。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | 单一渐变颜色。 |
| degree | double | 渐变的度数。取值范围为 0.0（暗）至 1.0（亮）。 |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype)。渐变阴影样式。 |
| variant | int | 渐变的变体。取值范围为 1 到 4，对应“填充效果”对话框中“渐变”选项卡上的四种变体之一。如果样式为 GradientStyle.FromCenter，则 Variant 参数只能为 1 或 2。 |

### setPresetColor(int value) {#setPresetColor-int-}
```
public void setPresetColor(int value)
```


返回指定填充的渐变预设颜色。适用于 Excel97-2003

参见 [GradientPresetType](../../com.aspose.cells/gradientpresettype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


将指定填充设置为预设颜色渐变。仅适用于 Excel 97-2003

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype)。预设颜色类型 |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype)。渐变阴影样式。 |
| variant | int | 渐变的变体。取值范围为 1 到 4，对应“填充效果”对话框中“渐变”选项卡上的四种变体之一。如果样式为 GradientStyle.FromCenter，则 Variant 参数只能为 1 或 2。 |

### setPresetThemeGradient(int gradientType, int themeColorType) {#setPresetThemeGradient-int-int-}
```
public void setPresetThemeGradient(int gradientType, int themeColorType)
```


设置预设主题渐变填充。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| gradientType | int | [PresetThemeGradientType](../../com.aspose.cells/presetthemegradienttype)。预设渐变类型。 |
| themeColorType | int | [ThemeColorType](../../com.aspose.cells/themecolortype)。主题颜色类型。 |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


将指定的填充设置为双色渐变。仅适用于 Excel 2007。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | 单一渐变颜色。 |
| color2 | [Color](../../com.aspose.cells/color) | 双色渐变。 |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype)。渐变阴影样式。 |
| variant | int | 渐变的变体。取值范围为 1 到 4，对应“填充效果”对话框中“渐变”选项卡上的四种变体之一。如果样式为 GradientStyle.FromCenter，则 Variant 参数只能为 1 或 2。 |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


将指定的填充设置为双色渐变。仅适用于 Excel 2007。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | 单一渐变颜色。 |
| transparency1 | double | color1 的透明度程度，取值范围为 0.0（不透明）至 1.0（透明）。 |
| color2 | [Color](../../com.aspose.cells/color) | 双色渐变。 |
| transparency2 | double | color2 的透明度程度，取值范围为 0.0（不透明）至 1.0（透明）。 |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype)。渐变阴影样式。 |
| variant | int | 渐变的变体。取值范围为 1 到 4，对应“填充效果”对话框中“渐变”选项卡上的四种变体之一。如果样式为 GradientStyle.FromCenter，则 Variant 参数只能为 1 或 2。 |

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

