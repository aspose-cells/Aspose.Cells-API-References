---
title: "CustomCommandButton"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 GridWeb 控件选项卡栏中的自定义命令按钮。"
type: docs
url: /zh/java/com.aspose.gridweb/customcommandbutton/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class CustomCommandButton extends Control
```

表示 GridWeb 控件选项卡栏中的自定义命令按钮。

**Example**

```
         GridWebBean GridWeb1=ExtPage.getInstance().getBean();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CustomCommandButton()](#CustomCommandButton--) | 默认构造函数。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getClientClickEvent()](#getClientClickEvent--) | 获取客户端的点击事件处理程序。 |
| [getCommand()](#getCommand--) | 获取命令名称。 |
| [getCommandType()](#getCommandType--) | 获取命令的渲染类型。 |
| [getDiscardInput()](#getDiscardInput--) | 指示当用户点击此按钮时是否在客户端浏览器中丢弃用户输入。 |
| [getImageUrl()](#getImageUrl--) | 获取命令按钮的图像 URL。 |
| [getText()](#getText--) | 获取命令按钮的替代文本。 |
| [getToolTip()](#getToolTip--) | 获取命令按钮的工具提示。 |
| [getUniqueID()](#getUniqueID--) | 获取控件中的唯一标识符。 |
| [getVisible()](#getVisible--) | 获取 Control 中的 Visible 属性。 |
| [getWidth()](#getWidth--) | 按钮的宽度。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setClientClickEvent(String value)](#setClientClickEvent-java.lang.String-) | 设置客户端的点击事件处理程序。 |
| [setCommand(String value)](#setCommand-java.lang.String-) | 设置命令名称。 |
| [setCommandType(int value)](#setCommandType-int-) | 设置命令的渲染类型。 |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | 指示当用户点击此按钮时是否在客户端浏览器中丢弃用户输入。 |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | 设置命令按钮的图像 URL。 |
| [setText(String value)](#setText-java.lang.String-) | 设置命令按钮的替代文本。 |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | 设置命令按钮的工具提示。 |
| [setVisible(boolean value)](#setVisible-boolean-) | 设置 Control 中的 Visible 属性。 |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | 按钮的宽度。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomCommandButton() {#CustomCommandButton--}
```
public CustomCommandButton()
```


默认构造函数。

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
### getClientClickEvent() {#getClientClickEvent--}
```
public String getClientClickEvent()
```


获取客户端的点击事件处理程序。

**Returns:**
java.lang.String
### getCommand() {#getCommand--}
```
public String getCommand()
```


获取命令名称。

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


获取命令的渲染类型。该类型可以是命令按钮或上下文菜单项。

参见 [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype)。

**Returns:**
int
### getDiscardInput() {#getDiscardInput--}
```
public boolean getDiscardInput()
```


指示当用户点击此按钮时是否在客户端浏览器中丢弃用户输入。可用作\"撤销\"操作。

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


获取命令按钮的图像 URL。如果设置为 null 或空字符串，按钮将仅显示其文本。

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


获取命令按钮的替代文本。

**Returns:**
java.lang.String
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


获取命令按钮的工具提示。

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


获取控件中的唯一标识符。

**Returns:**
java.lang.String
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


获取 Control 中的 Visible 属性。

**Returns:**
boolean
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


按钮的宽度。

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
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




### setClientClickEvent(String value) {#setClientClickEvent-java.lang.String-}
```
public void setClientClickEvent(String value)
```


设置客户端的点击事件处理程序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


设置命令名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


设置命令的渲染类型。该类型可以是命令按钮或上下文菜单项。

参见 [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```


指示当用户点击此按钮时是否在客户端浏览器中丢弃用户输入。可用作\"撤销\"操作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


设置命令按钮的图像 URL。如果设置为 null 或空字符串，按钮将仅显示其文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


设置命令按钮的替代文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


设置命令按钮的工具提示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


设置 Control 中的 Visible 属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


按钮的宽度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

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

