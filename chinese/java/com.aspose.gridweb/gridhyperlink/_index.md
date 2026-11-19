---
title: "GridHyperlink"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示超链接的对象。"
type: docs
url: /zh/java/com.aspose.gridweb/gridhyperlink/
---

**Inheritance:**
java.lang.Object
```
public class GridHyperlink
```

封装表示超链接的对象。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddress()](#getAddress--) | 表示超链接的地址。 |
| [getAltText()](#getAltText--) | 获取图像链接的替代文本，请注意这是一个扩展属性，不能保存在 Excel 文件中。 |
| [getArea()](#getArea--) | 获取超链接的范围。 |
| [getClass()](#getClass--) |  |
| [getCommand()](#getCommand--) | 返回或设置指定超链接的自定义命令值文本。 |
| [getDiscardInput()](#getDiscardInput--) | 指示在用户点击此 CellCommand 超链接时，是否在客户端浏览器中丢弃用户输入。 |
| [getImageURL()](#getImageURL--) | 获取链接的图像 URL，超链接中没有 imageurl 属性，因此实际使用 TextToDisplay 来记录此值，TextToDisplay 将被设置为 <img src=value>，从而更改 TextToDisplay 的值。 |
| [getScreenTip()](#getScreenTip--) | 返回或设置指定超链接的屏幕提示文本。 |
| [getTarget()](#getTarget--) | 获取网页链接的目标类型，请注意这是一个扩展属性，不能保存在 Excel 文件中。 |
| [getTextToDisplay()](#getTextToDisplay--) | 表示指定超链接要显示的文本。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddress(String value)](#setAddress-java.lang.String-) | 表示超链接的地址。 |
| [setAltText(String value)](#setAltText-java.lang.String-) | 设置图像链接的替代文本，请注意这是一个扩展属性，不能保存在 Excel 文件中。 |
| [setCommand(String value)](#setCommand-java.lang.String-) | 返回或设置指定超链接的自定义命令值文本。 |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | 指示在用户点击此 CellCommand 超链接时，是否在客户端浏览器中丢弃用户输入。 |
| [setImageURL(String value)](#setImageURL-java.lang.String-) | 设置链接的图像 URL，超链接中没有 imageurl 属性，因此实际使用 TextToDisplay 来记录此值，TextToDisplay 将被设置为 <img src=value>，从而更改 TextToDisplay 的值。 |
| [setScreenTip(String value)](#setScreenTip-java.lang.String-) | 返回或设置指定超链接的屏幕提示文本。 |
| [setTarget(String value)](#setTarget-java.lang.String-) | 设置网页链接的目标类型，请注意这是一个扩展属性，不能保存在 Excel 文件中。 |
| [setTextToDisplay(String value)](#setTextToDisplay-java.lang.String-) | 表示指定超链接要显示的文本。 |
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
### getAddress() {#getAddress--}
```
public String getAddress()
```


表示超链接的地址。

**Returns:**
java.lang.String
### getAltText() {#getAltText--}
```
public String getAltText()
```


获取图像链接的替代文本，请注意这是一个扩展属性，不能保存在 Excel 文件中。

**Returns:**
java.lang.String
### getArea() {#getArea--}
```
public GridCellArea getArea()
```


获取超链接的范围。

**Returns:**
[GridCellArea](../../com.aspose.gridweb/gridcellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCommand() {#getCommand--}
```
public String getCommand()
```


返回或设置指定超链接的自定义命令值文本。

**Returns:**
java.lang.String
### getDiscardInput() {#getDiscardInput--}
```
public boolean getDiscardInput()
```


指示在用户点击此 CellCommand 超链接时，是否在客户端浏览器中丢弃用户输入。可用作“撤销”操作。

**Returns:**
boolean
### getImageURL() {#getImageURL--}
```
public String getImageURL()
```


获取链接的图像 URL，超链接中没有 imageurl 属性，因此实际使用 TextToDisplay 来记录此值，TextToDisplay 将被设置为 <img src=value>，从而更改 TextToDisplay 的值。

**Returns:**
java.lang.String
### getScreenTip() {#getScreenTip--}
```
public String getScreenTip()
```


返回或设置指定超链接的屏幕提示文本。

**Returns:**
java.lang.String
### getTarget() {#getTarget--}
```
public String getTarget()
```


获取网页链接的目标类型，请注意这是一个扩展属性，不能保存在 Excel 文件中。

**Returns:**
java.lang.String
### getTextToDisplay() {#getTextToDisplay--}
```
public String getTextToDisplay()
```


表示指定超链接要显示的文本。默认值是超链接的地址。

**Returns:**
java.lang.String
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




### setAddress(String value) {#setAddress-java.lang.String-}
```
public void setAddress(String value)
```


表示超链接的地址。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setAltText(String value) {#setAltText-java.lang.String-}
```
public void setAltText(String value)
```


设置图像链接的替代文本，请注意这是一个扩展属性，不能保存在 Excel 文件中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


返回或设置指定超链接的自定义命令值文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```


指示在用户点击此 CellCommand 超链接时，是否在客户端浏览器中丢弃用户输入。可用作“撤销”操作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setImageURL(String value) {#setImageURL-java.lang.String-}
```
public void setImageURL(String value)
```


设置链接的图像 URL，超链接中没有 imageurl 属性，因此实际使用 TextToDisplay 来记录此值，TextToDisplay 将被设置为 <img src=value>，从而更改 TextToDisplay 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setScreenTip(String value) {#setScreenTip-java.lang.String-}
```
public void setScreenTip(String value)
```


返回或设置指定超链接的屏幕提示文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTarget(String value) {#setTarget-java.lang.String-}
```
public void setTarget(String value)
```


设置网页链接的目标类型，请注意这是一个扩展属性，不能保存在 Excel 文件中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTextToDisplay(String value) {#setTextToDisplay-java.lang.String-}
```
public void setTextToDisplay(String value)
```


表示指定超链接要显示的文本。默认值是超链接的地址。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

