---
title: "RenderingWatermark"
second_title: "Aspose.Cells for Java API 参考"
description: "用于渲染的水印。"
type: docs
url: /zh/java/com.aspose.cells/renderingwatermark/
---

**Inheritance:**
java.lang.Object
```
public class RenderingWatermark
```

用于渲染的水印。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [RenderingWatermark(String text, RenderingFont renderingFont)](#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-) | 创建文本水印的实例。 |
| [RenderingWatermark(byte[] imageData)](#RenderingWatermark-byte---) | 创建图像水印的实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | 获取水印的字体。 |
| [getHAlignment()](#getHAlignment--) | 获取水印相对于页面的水平对齐方式。 |
| [getImage()](#getImage--) | 获取水印的图像。 |
| [getOffsetX()](#getOffsetX--) | 获取相对于 [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) 的偏移值。 |
| [getOffsetY()](#getOffsetY--) | 获取相对于 [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) 的偏移值。 |
| [getOpacity()](#getOpacity--) | 获取水印的透明度，范围为 [0, 1]。 |
| [getRotation()](#getRotation--) | 获取水印的旋转角度（单位：度）。 |
| [getScaleToPagePercent()](#getScaleToPagePercent--) | 获取相对于目标页面的比例（百分比）。 |
| [getText()](#getText--) | 获取水印的文本。 |
| [getVAlignment()](#getVAlignment--) | 获取水印相对于页面的垂直对齐方式。 |
| [hashCode()](#hashCode--) |  |
| [isBackground()](#isBackground--) | 指示水印是否放置在页面内容后面。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackground(boolean value)](#setBackground-boolean-) | 指示水印是否放置在页面内容后面。 |
| [setHAlignment(int value)](#setHAlignment-int-) | 设置水印相对于页面的水平对齐方式。 |
| [setOffsetX(float value)](#setOffsetX-float-) | 设置偏移值为 [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [setOffsetY(float value)](#setOffsetY-float-) | 设置偏移值为 [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [setOpacity(float value)](#setOpacity-float-) | 设置水印的不透明度，范围为 [0, 1]。 |
| [setRotation(float value)](#setRotation-float-) | 设置水印的旋转角度（度）。 |
| [setScaleToPagePercent(int value)](#setScaleToPagePercent-int-) | 设置相对于目标页面的比例（百分比）。 |
| [setVAlignment(int value)](#setVAlignment-int-) | 设置水印相对于页面的垂直对齐方式。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### RenderingWatermark(String text, RenderingFont renderingFont) {#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-}
```
public RenderingWatermark(String text, RenderingFont renderingFont)
```


创建文本水印的实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文本 | java.lang.String | 水印文本 |
| renderingFont | [RenderingFont](../../com.aspose.cells/renderingfont) | 水印字体 |

### RenderingWatermark(byte[] imageData) {#RenderingWatermark-byte---}
```
public RenderingWatermark(byte[] imageData)
```


创建图像水印的实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| imageData | byte[] |  |

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
### getFont() {#getFont--}
```
public RenderingFont getFont()
```


获取水印的字体。

**Returns:**
[RenderingFont](../../com.aspose.cells/renderingfont)
### getHAlignment() {#getHAlignment--}
```
public int getHAlignment()
```


获取水印相对于页面的水平对齐方式。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Remarks**

仅 Left、Center、Right 有效。默认是 Left。

**Returns:**
int
### getImage() {#getImage--}
```
public byte[] getImage()
```


获取水印的图像。

**Returns:**
byte[]
### getOffsetX() {#getOffsetX--}
```
public float getOffsetX()
```


获取相对于 [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) 的偏移值。

**Returns:**
float
### getOffsetY() {#getOffsetY--}
```
public float getOffsetY()
```


获取相对于 [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) 的偏移值。

**Returns:**
float
### getOpacity() {#getOpacity--}
```
public float getOpacity()
```


获取水印的透明度，范围为 [0, 1]。

**Returns:**
float
### getRotation() {#getRotation--}
```
public float getRotation()
```


获取水印的旋转角度（单位：度）。

**Returns:**
float
### getScaleToPagePercent() {#getScaleToPagePercent--}
```
public int getScaleToPagePercent()
```


获取相对于目标页面的比例（百分比）。

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


获取水印的文本。

**Returns:**
java.lang.String
### getVAlignment() {#getVAlignment--}
```
public int getVAlignment()
```


获取水印相对于页面的垂直对齐方式。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Remarks**

仅 Top、Center、Bottom 有效。默认是 Top。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBackground() {#isBackground--}
```
public boolean isBackground()
```


指示水印是否放置在页面内容后面。

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




### setBackground(boolean value) {#setBackground-boolean-}
```
public void setBackground(boolean value)
```


指示水印是否放置在页面内容后面。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHAlignment(int value) {#setHAlignment-int-}
```
public void setHAlignment(int value)
```


设置水印相对于页面的水平对齐方式。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Remarks**

仅 Left、Center、Right 有效。默认是 Left。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setOffsetX(float value) {#setOffsetX-float-}
```
public void setOffsetX(float value)
```


设置偏移值为 [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setOffsetY(float value) {#setOffsetY-float-}
```
public void setOffsetY(float value)
```


设置偏移值为 [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setOpacity(float value) {#setOpacity-float-}
```
public void setOpacity(float value)
```


设置水印的不透明度，范围为 [0, 1]。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setRotation(float value) {#setRotation-float-}
```
public void setRotation(float value)
```


设置水印的旋转角度（度）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setScaleToPagePercent(int value) {#setScaleToPagePercent-int-}
```
public void setScaleToPagePercent(int value)
```


设置相对于目标页面的比例（百分比）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setVAlignment(int value) {#setVAlignment-int-}
```
public void setVAlignment(int value)
```


设置水印相对于页面的垂直对齐方式。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Remarks**

仅 Top、Center、Bottom 有效。默认是 Top。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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

