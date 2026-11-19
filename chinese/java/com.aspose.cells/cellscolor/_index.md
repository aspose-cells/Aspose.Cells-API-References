---
title: "CellsColor"
second_title: "Aspose.Cells for Java API 参考"
description: "表示所有类型的颜色。"
type: docs
url: /zh/java/com.aspose.cells/cellscolor/
---

**Inheritance:**
java.lang.Object
```
public class CellsColor
```

表示所有类型的颜色。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgb()](#getArgb--) | 从 32 位 ARGB 值获取颜色。 |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | 获取 RGB 颜色。 |
| [getColorIndex()](#getColorIndex--) | 获取调色板中的颜色索引。 |
| [getThemeColor()](#getThemeColor--) | 获取主题颜色。 |
| [getTransparency()](#getTransparency--) | 获取透明度，取值范围为 0.0（不透明）至 1.0（透明）。 |
| [getType()](#getType--) | 颜色类型。 |
| [hashCode()](#hashCode--) |  |
| [isShapeColor()](#isShapeColor--) | 获取应应用于单元格或形状的颜色。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgb(int value)](#setArgb-int-) | 从 32 位 ARGB 值设置颜色。 |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | 设置 RGB 颜色。 |
| [setColorIndex(int value)](#setColorIndex-int-) | 在调色板中设置颜色索引。 |
| [setShapeColor(boolean value)](#setShapeColor-boolean-) | 设置应应用于单元格或形状的颜色。 |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | 获取主题颜色。 |
| [setTintOfShapeColor(double tint)](#setTintOfShapeColor-double-) | 设置形状颜色的色调 |
| [setTransparency(double value)](#setTransparency-double-) | 设置透明度，取值范围为 0.0（不透明）至 1.0（透明）。 |
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
### getArgb() {#getArgb--}
```
public int getArgb()
```


从 32 位 ARGB 值获取颜色。

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


获取 RGB 颜色。

**Returns:**
[Color](../../com.aspose.cells/color)
### getColorIndex() {#getColorIndex--}
```
public int getColorIndex()
```


获取调色板中的颜色索引。仅适用于索引颜色。

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


获取主题颜色。仅适用于主题颜色类型。

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


获取透明度，取值范围为 0.0（不透明）至 1.0（透明）。

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


颜色类型。

参见 [ColorType](../../com.aspose.cells/colortype)。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isShapeColor() {#isShapeColor--}
```
public boolean isShapeColor()
```


获取应应用于单元格或形状的颜色。

**Remarks**

单元格和形状的颜色表达不同。例如：相同色调值的主题颜色在单元格和形状中会不同。

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




### setArgb(int value) {#setArgb-int-}
```
public void setArgb(int value)
```


从 32 位 ARGB 值设置颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


设置 RGB 颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setColorIndex(int value) {#setColorIndex-int-}
```
public void setColorIndex(int value)
```


在调色板中设置颜色索引。仅适用于索引颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setShapeColor(boolean value) {#setShapeColor-boolean-}
```
public void setShapeColor(boolean value)
```


设置应应用于单元格或形状的颜色。

**Remarks**

单元格和形状的颜色表达不同。例如：相同色调值的主题颜色在单元格和形状中会不同。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


获取主题颜色。仅适用于主题颜色类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTintOfShapeColor(double tint) {#setTintOfShapeColor-double-}
```
public void setTintOfShapeColor(double tint)
```


设置形状颜色的色调

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tint | double |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


设置透明度，取值范围为 0.0（不透明）至 1.0（透明）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

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

