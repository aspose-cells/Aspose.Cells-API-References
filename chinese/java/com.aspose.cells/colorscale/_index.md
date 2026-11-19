---
title: "ColorScale"
second_title: "Aspose.Cells for Java API 参考"
description: "描述 ColorScale 条件格式规则。"
type: docs
url: /zh/java/com.aspose.cells/colorscale/
---

**Inheritance:**
java.lang.Object
```
public class ColorScale
```

描述 ColorScale 条件格式规则。此条件格式规则在单元格上创建渐变色标。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getIs3ColorScale()](#getIs3ColorScale--) | 指示条件格式是否为三色标度。 |
| [getMaxCfvo()](#getMaxCfvo--) | 获取此 ColorScale 的最大值对象。 |
| [getMaxColor()](#getMaxColor--) | 获取范围内最大值的渐变颜色。 |
| [getMidCfvo()](#getMidCfvo--) | 获取此 ColorScale 的中间值对象。 |
| [getMidColor()](#getMidColor--) | 获取范围内中间值的渐变颜色。 |
| [getMinCfvo()](#getMinCfvo--) | 获取此 ColorScale 的最小值对象。 |
| [getMinColor()](#getMinColor--) | 获取范围内最小值的渐变颜色。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setIs3ColorScale(boolean value)](#setIs3ColorScale-boolean-) | 指示条件格式是否为三色标度。 |
| [setMaxColor(Color value)](#setMaxColor-com.aspose.cells.Color-) | 设置范围内最大值的渐变颜色。 |
| [setMidColor(Color value)](#setMidColor-com.aspose.cells.Color-) | 设置范围内中间值的渐变颜色。 |
| [setMinColor(Color value)](#setMinColor-com.aspose.cells.Color-) | 设置范围内最小值的渐变颜色。 |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getIs3ColorScale() {#getIs3ColorScale--}
```
public boolean getIs3ColorScale()
```


指示条件格式是否为三色标度。

**Returns:**
boolean
### getMaxCfvo() {#getMaxCfvo--}
```
public ConditionalFormattingValue getMaxCfvo()
```


获取此 ColorScale 的最大值对象。不能将 null 或类型为 FormatConditionValueType.Min 的 CFValueObject 设置为它。

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMaxColor() {#getMaxColor--}
```
public Color getMaxColor()
```


获取范围内最大值的渐变颜色。

**Returns:**
[Color](../../com.aspose.cells/color)
### getMidCfvo() {#getMidCfvo--}
```
public ConditionalFormattingValue getMidCfvo()
```


获取此 ColorScale 的中间值对象。不能将类型为 FormatConditionValueType.Max 或 FormatConditionValueType.Min 的 CFValueObject 设置为它。

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMidColor() {#getMidColor--}
```
public Color getMidColor()
```


获取范围内中间值的渐变颜色。

**Returns:**
[Color](../../com.aspose.cells/color)
### getMinCfvo() {#getMinCfvo--}
```
public ConditionalFormattingValue getMinCfvo()
```


获取此 ColorScale 的最小值对象。不能将 null 或类型为 FormatConditionValueType.Max 的 CFValueObject 设置为它。

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMinColor() {#getMinColor--}
```
public Color getMinColor()
```


获取范围内最小值的渐变颜色。

**Returns:**
[Color](../../com.aspose.cells/color)
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




### setIs3ColorScale(boolean value) {#setIs3ColorScale-boolean-}
```
public void setIs3ColorScale(boolean value)
```


指示条件格式是否为三色标度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMaxColor(Color value) {#setMaxColor-com.aspose.cells.Color-}
```
public void setMaxColor(Color value)
```


设置范围内最大值的渐变颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setMidColor(Color value) {#setMidColor-com.aspose.cells.Color-}
```
public void setMidColor(Color value)
```


设置范围内中间值的渐变颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setMinColor(Color value) {#setMinColor-com.aspose.cells.Color-}
```
public void setMinColor(Color value)
```


设置范围内最小值的渐变颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

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

