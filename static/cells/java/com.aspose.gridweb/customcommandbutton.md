##CustomCommandButton
Represents a custom command button in the tab bar of the GridWeb control.
**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class CustomCommandButton extends Control
```
Represents a custom command button in the tab bar of the GridWeb control.
**Example**
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
| [getClientClickEvent()](#getClientClickEvent--) | Gets the click event handler at client side. |
| [getCommand()](#getCommand--) | Gets the command name. |
| [getCommandType()](#getCommandType--) | Gets the rendering type of the command. |
| [getDiscardInput()](#getDiscardInput--) | Indicates whether to discard user input at client browser when user click this button. |
| [getImageUrl()](#getImageUrl--) | Gets the command button's image url. |
| [getText()](#getText--) | Gets the alternative text of the command button. |
| [getToolTip()](#getToolTip--) | Gets the tooltip of the command button. |
| [getUniqueID()](#getUniqueID--) | Gets the UniqueID in the Control |
| [getVisible()](#getVisible--) | Gets the Visible in the Control |
| [getWidth()](#getWidth--) | Width of the button. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setClientClickEvent(String value)](#setClientClickEvent-java.lang.String-) | Sets the click event handler at client side. |
| [setCommand(String value)](#setCommand-java.lang.String-) | Sets the command name. |
| [setCommandType(int value)](#setCommandType-int-) | Sets the rendering type of the command. |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | Indicates whether to discard user input at client browser when user click this button. |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | Sets the command button's image url. |
| [setText(String value)](#setText-java.lang.String-) | Sets the alternative text of the command button. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | Sets the tooltip of the command button. |
| [setVisible(boolean value)](#setVisible-boolean-) | Sets the Visible in the Control |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Width of the button. |
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
Gets the click event handler at client side.
**Returns:**
java.lang.String
### getCommand() {#getCommand--}
```
public String getCommand()
```
Gets the command name.
**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```
Gets the rendering type of the command. The type can be command button or context menu item.
See [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).
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
Gets the command button's image url. If sets to null or empty string, the button will only display it's text.
**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```
Gets the alternative text of the command button.
**Returns:**
java.lang.String
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```
Gets the tooltip of the command button.
**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```
Gets the UniqueID in the Control
**Returns:**
java.lang.String
### getVisible() {#getVisible--}
```
public boolean getVisible()
```
Gets the Visible in the Control
**Returns:**
boolean
### getWidth() {#getWidth--}
```
public Unit getWidth()
```
Width of the button.
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
Sets the click event handler at client side.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```
Sets the command name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```
Sets the rendering type of the command. The type can be command button or context menu item.
See [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```
Indicates whether to discard user input at client browser when user click this button. Could be used as an "undo" action.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```
Sets the command button's image url. If sets to null or empty string, the button will only display it's text.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```
Sets the alternative text of the command button.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```
Sets the tooltip of the command button.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```
Sets the Visible in the Control
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```
Width of the button.
**Parameters:**
| Parameter | Type | Description |
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
