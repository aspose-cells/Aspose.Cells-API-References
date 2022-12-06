---
title: CustomCommandButton
second_title: Aspose.Cells for Java API Reference
description: Represents a custom command button in the tab bar of the GridWeb control.
type: docs
url: /java/com.aspose.gridweb/customcommandbutton/
---

**Inheritance:**
java.lang.Object
```
public class CustomCommandButton
```

Represents a custom command button in the tab bar of the GridWeb control.

```
GridWebBean GridWeb1=ExtPage.getInstance().getBean();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## Constructors

| Constructor | Description |
| --- | --- |
| [CustomCommandButton()](#CustomCommandButton--) | Default constructor. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getClientClickEvent()](#getClientClickEvent--) | the click event handler at client side. |
| [getCommand()](#getCommand--) | the command name. |
| [getCommandType()](#getCommandType--) | the rendering type of the command. |
| [getDiscardInput()](#getDiscardInput--) | Indicates whether to discard user input at client browser when user click this button. |
| [getImageUrl()](#getImageUrl--) | the command button's image url. |
| [getText()](#getText--) | the alternative text of the command button. |
| [getToolTip()](#getToolTip--) | the tooltip of the command button. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setClientClickEvent(String value)](#setClientClickEvent-java.lang.String-) | For the description of this property, please see [getClientClickEvent()](../../com.aspose.gridweb/customcommandbutton\#getClientClickEvent--) |
| [setCommand(String value)](#setCommand-java.lang.String-) | For the description of this property, please see [getCommand()](../../com.aspose.gridweb/customcommandbutton\#getCommand--) |
| [setCommandType(int value)](#setCommandType-int-) | For the description of this property, please see [getCommandType()](../../com.aspose.gridweb/customcommandbutton\#getCommandType--) |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | For the description of this property, please see [getDiscardInput()](../../com.aspose.gridweb/customcommandbutton\#getDiscardInput--) |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | For the description of this property, please see [getImageUrl()](../../com.aspose.gridweb/customcommandbutton\#getImageUrl--) |
| [setText(String value)](#setText-java.lang.String-) | For the description of this property, please see [getText()](../../com.aspose.gridweb/customcommandbutton\#getText--) |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | For the description of this property, please see [getToolTip()](../../com.aspose.gridweb/customcommandbutton\#getToolTip--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomCommandButton() {#CustomCommandButton--}
```
public CustomCommandButton()
```


Default constructor.

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
### getClientClickEvent() {#getClientClickEvent--}
```
public String getClientClickEvent()
```


the click event handler at client side.

**Returns:**
java.lang.String
### getCommand() {#getCommand--}
```
public String getCommand()
```


the command name.

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


the rendering type of the command. The type can be command button or context menu item.

**Returns:**
int
### getDiscardInput() {#getDiscardInput--}
```
public boolean getDiscardInput()
```


Indicates whether to discard user input at client browser when user click this button. Could be used as an "undo" action.

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


the command button's image url. If sets to null or empty string, the button will only display it's text.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


the alternative text of the command button.

**Returns:**
java.lang.String
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


the tooltip of the command button.

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




### setClientClickEvent(String value) {#setClientClickEvent-java.lang.String-}
```
public void setClientClickEvent(String value)
```


For the description of this property, please see [getClientClickEvent()](../../com.aspose.gridweb/customcommandbutton\#getClientClickEvent--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


For the description of this property, please see [getCommand()](../../com.aspose.gridweb/customcommandbutton\#getCommand--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


For the description of this property, please see [getCommandType()](../../com.aspose.gridweb/customcommandbutton\#getCommandType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```


For the description of this property, please see [getDiscardInput()](../../com.aspose.gridweb/customcommandbutton\#getDiscardInput--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


For the description of this property, please see [getImageUrl()](../../com.aspose.gridweb/customcommandbutton\#getImageUrl--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


For the description of this property, please see [getText()](../../com.aspose.gridweb/customcommandbutton\#getText--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


For the description of this property, please see [getToolTip()](../../com.aspose.gridweb/customcommandbutton\#getToolTip--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

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

