---
title: "TickLabels"
second_title: "Aspose.Cells for Java API 参考"
description: "表示与图表轴上刻度线关联的刻度标记标签。"
type: docs
url: /zh/java/com.aspose.cells/ticklabels/
---

**Inheritance:**
java.lang.Object
```
public class TickLabels
```

表示与图表轴上刻度线关联的刻度标记标签。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignmentType()](#getAlignmentType--) | 获取轴上刻度标签的文本对齐方式。 |
| [getAutoScaleFont()](#getAutoScaleFont--) | 如果对象中的文本在对象大小变化时会更改字体大小，则为 True。 |
| [getBackgroundMode()](#getBackgroundMode--) | 获取背景的显示模式 |
| [getClass()](#getClass--) |  |
| [getDirectionType()](#getDirectionType--) | 获取文本的方向。 |
| [getDisplayNumberFormat()](#getDisplayNumberFormat--) | 获取刻度标签的显示数字格式。 |
| [getFont()](#getFont--) | 返回一个 [getFont()](../../com.aspose.cells/ticklabels\#getFont--) 对象，表示指定 TickLabels 对象的字体。 |
| [getNumber()](#getNumber--) | 表示 TickLabels 对象的格式数字。 |
| [getNumberFormat()](#getNumberFormat--) | 表示 TickLabels 对象的格式字符串。 |
| [getNumberFormatLinked()](#getNumberFormatLinked--) | 如果数字格式与单元格关联，则为 true（这样当单元格的数字格式更改时，标签中的数字格式也会随之更改）。 |
| [getOffset()](#getOffset--) | 获取标签距离类别轴的距离。 |
| [getReadingOrder()](#getReadingOrder--) | 表示文本阅读顺序。 |
| [getRotationAngle()](#getRotationAngle--) | 表示顺时针的文本旋转角度。 |
| [getTextDirection()](#getTextDirection--) | 表示文本阅读顺序。 |
| [getTickLabelItems()](#getTickLabelItems--) | 获取轴的显示刻度标签。 |
| [hashCode()](#hashCode--) |  |
| [isAutomaticRotation()](#isAutomaticRotation--) | 指示旋转角度是否自动。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentType(int value)](#setAlignmentType-int-) | 设置轴上刻度标签的文本对齐方式。 |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | 如果对象中的文本在对象大小变化时会更改字体大小，则为 True。 |
| [setAutomaticRotation(boolean value)](#setAutomaticRotation-boolean-) | 指示旋转角度是否自动。 |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | 设置背景的显示模式 |
| [setDirectionType(int value)](#setDirectionType-int-) | 设置文本的方向。 |
| [setNumber(int value)](#setNumber-int-) | 表示 TickLabels 对象的格式数字。 |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | 表示 TickLabels 对象的格式字符串。 |
| [setNumberFormatLinked(boolean value)](#setNumberFormatLinked-boolean-) | 如果数字格式与单元格关联，则为 true（这样当单元格的数字格式更改时，标签中的数字格式也会随之更改）。 |
| [setOffset(int value)](#setOffset-int-) | 设置标签与分类轴之间的距离。 |
| [setReadingOrder(int value)](#setReadingOrder-int-) | 表示文本阅读顺序。 |
| [setRotationAngle(int value)](#setRotationAngle-int-) | 表示顺时针的文本旋转角度。 |
| [setTextDirection(int value)](#setTextDirection-int-) | 表示文本阅读顺序。 |
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
### getAlignmentType() {#getAlignmentType--}
```
public int getAlignmentType()
```


获取轴上刻度标签的文本对齐方式。

参见 [TickLabelAlignmentType](../../com.aspose.cells/ticklabelalignmenttype)。

**Returns:**
int
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


如果对象中的文本在对象大小变化时会更改字体大小，则为 True。默认值为 True。

**Returns:**
boolean
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


获取背景的显示模式

参见 [BackgroundMode](../../com.aspose.cells/backgroundmode)。

**Returns:**
int
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


获取文本的方向。

参见 [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype)。

**Returns:**
int
### getDisplayNumberFormat() {#getDisplayNumberFormat--}
```
public String getDisplayNumberFormat()
```


获取刻度标签的显示数字格式。

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public Font getFont()
```


返回一个 [getFont()](../../com.aspose.cells/ticklabels\#getFont--) 对象，表示指定 TickLabels 对象的字体。

**Returns:**
[Font](../../com.aspose.cells/font)
### getNumber() {#getNumber--}
```
public int getNumber()
```


表示 TickLabels 对象的格式数字。

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


表示 TickLabels 对象的格式字符串。

**Remarks**

格式字符串与单元格的自定义格式字符串设置相同。例如，"$0"。

**Returns:**
java.lang.String
### getNumberFormatLinked() {#getNumberFormatLinked--}
```
public boolean getNumberFormatLinked()
```


如果数字格式与单元格关联，则为 true（这样当单元格的数字格式更改时，标签中的数字格式也会随之更改）。

**Returns:**
boolean
### getOffset() {#getOffset--}
```
public int getOffset()
```


获取标签与分类轴之间的距离。仅适用于分类（x）轴。

**Remarks**

默认距离为 100%，表示轴标签与轴线之间的默认间距。该值可以是相对于轴标签字体大小的 0 到 1000 的整数百分比。

**Returns:**
int
### getReadingOrder() {#getReadingOrder--}
```
public int getReadingOrder()
```


表示文本阅读顺序。

参见 [TextDirectionType](../../com.aspose.cells/textdirectiontype)。

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


表示顺时针的文本旋转角度。

**Remarks**


0：未旋转。

255：从上到下。

\-90：向下。

90：向上。


**Returns:**
int
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


表示文本阅读顺序。

参见 [TextDirectionType](../../com.aspose.cells/textdirectiontype)。

**Remarks**

注意：此成员已过时。请改用 TickLabels.ReadingOrder 属性。此属性将在自 2020 年 3 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getTickLabelItems() {#getTickLabelItems--}
```
public TickLabelItem[] getTickLabelItems()
```


获取轴的显示刻度标签。

**Remarks**

仅在调用 [Chart.calculate()](../../com.aspose.cells/chart\#calculate--) 方法后可用。

**Returns:**
com.aspose.cells.TickLabelItem[]
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutomaticRotation() {#isAutomaticRotation--}
```
public boolean isAutomaticRotation()
```


指示旋转角度是否自动。

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




### setAlignmentType(int value) {#setAlignmentType-int-}
```
public void setAlignmentType(int value)
```


设置轴上刻度标签的文本对齐方式。

参见 [TickLabelAlignmentType](../../com.aspose.cells/ticklabelalignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


如果对象中的文本在对象大小变化时会更改字体大小，则为 True。默认值为 True。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutomaticRotation(boolean value) {#setAutomaticRotation-boolean-}
```
public void setAutomaticRotation(boolean value)
```


指示旋转角度是否自动。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


设置背景的显示模式

参见 [BackgroundMode](../../com.aspose.cells/backgroundmode)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDirectionType(int value) {#setDirectionType-int-}
```
public void setDirectionType(int value)
```


设置文本的方向。

参见 [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


表示 TickLabels 对象的格式数字。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


表示 TickLabels 对象的格式字符串。

**Remarks**

格式字符串与单元格的自定义格式字符串设置相同。例如，"$0"。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setNumberFormatLinked(boolean value) {#setNumberFormatLinked-boolean-}
```
public void setNumberFormatLinked(boolean value)
```


如果数字格式与单元格关联，则为 true（这样当单元格的数字格式更改时，标签中的数字格式也会随之更改）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOffset(int value) {#setOffset-int-}
```
public void setOffset(int value)
```


设置标签与分类轴之间的距离。仅适用于分类（x）轴。

**Remarks**

默认距离为 100%，表示轴标签与轴线之间的默认间距。该值可以是相对于轴标签字体大小的 0 到 1000 的整数百分比。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setReadingOrder(int value) {#setReadingOrder-int-}
```
public void setReadingOrder(int value)
```


表示文本阅读顺序。

参见 [TextDirectionType](../../com.aspose.cells/textdirectiontype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


表示顺时针的文本旋转角度。

**Remarks**


0：未旋转。

255：从上到下。

\-90：向下。

90：向上。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


表示文本阅读顺序。

参见 [TextDirectionType](../../com.aspose.cells/textdirectiontype)。

**Remarks**

注意：此成员已过时。请改用 TickLabels.ReadingOrder 属性。此属性将在自 2020 年 3 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

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

