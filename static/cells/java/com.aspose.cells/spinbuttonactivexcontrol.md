##SpinButtonActiveXControl
Represents the SpinButton control.
**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class SpinButtonActiveXControl extends ActiveXControl
```
Represents the SpinButton control.
**Example**
```
//Initialize a new workbook.
Workbook book = new Workbook();
//Add a ToggleButtonActiveXControl.
Shape shape = book.getWorksheets().get(0).getShapes().addActiveXControl(ControlType.SPIN_BUTTON, 1, 0, 1, 0, 100, 50);
SpinButtonActiveXControl activeXControl = (SpinButtonActiveXControl)shape.getActiveXControl();
//do your business
//Save the excel file.
book.save("exmaple.xlsx");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Gets the ole color of the background. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Gets the binary data of the control. |
| [getFont()](#getFont--) | Represents the font of the control. |
| [getForeOleColor()](#getForeOleColor--) | Gets the ole color of the foreground. |
| [getHeight()](#getHeight--) | Gets the height of the control in unit of points. |
| [getIMEMode()](#getIMEMode--) | Gets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [getLinkedCell()](#getLinkedCell--) | Gets the linked cell. |
| [getListFillRange()](#getListFillRange--) | Gets the list fill range. |
| [getMax()](#getMax--) | Gets the maximum acceptable value. |
| [getMin()](#getMin--) | Gets the minimum acceptable value. |
| [getMouseIcon()](#getMouseIcon--) | Gets a custom icon to display as the mouse pointer for the control. |
| [getMousePointer()](#getMousePointer--) | Gets the type of icon displayed as the mouse pointer for the control. |
| [getOrientation()](#getOrientation--) | Gets whether the SpinButton or ScrollBar is oriented vertically or horizontally. |
| [getPosition()](#getPosition--) | Gets the value. |
| [getShadow()](#getShadow--) | Indicates whether to show a shadow. |
| [getSmallChange()](#getSmallChange--) | Gets the amount by which the Position property changes |
| [getTextAlign()](#getTextAlign--) | Represents how to align the text used by the control. |
| [getType()](#getType--) | Gets the type of the ActiveX control. |
| [getWidth()](#getWidth--) | Gets the width of the control in unit of points. |
| [getWorkbook()](#getWorkbook--) | Gets the [Workbook](../../com.aspose.cells/workbook) object. |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Indicates whether the control will automatically resize to display its entire contents. |
| [isEnabled()](#isEnabled--) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [isLocked()](#isLocked--) | Indicates whether data in the control is locked for editing. |
| [isTransparent()](#isTransparent--) | Indicates whether the control is transparent. |
| [isVisible()](#isVisible--) | Indicates whether this control is visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indicates whether the control will automatically resize to display its entire contents. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Sets the ole color of the background. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Sets the ole color of the foreground. |
| [setHeight(double value)](#setHeight-double-) | Sets the height of the control in unit of points. |
| [setIMEMode(int value)](#setIMEMode-int-) | Sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Sets the linked cell. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Sets the list fill range. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indicates whether data in the control is locked for editing. |
| [setMax(int value)](#setMax-int-) | Sets the maximum acceptable value. |
| [setMin(int value)](#setMin-int-) | Sets the minimum acceptable value. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Sets a custom icon to display as the mouse pointer for the control. |
| [setMousePointer(int value)](#setMousePointer-int-) | Sets the type of icon displayed as the mouse pointer for the control. |
| [setOrientation(int value)](#setOrientation-int-) | Sets whether the SpinButton or ScrollBar is oriented vertically or horizontally. |
| [setPosition(int value)](#setPosition-int-) | Sets the value. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indicates whether to show a shadow. |
| [setSmallChange(int value)](#setSmallChange-int-) | Sets the amount by which the Position property changes |
| [setTextAlign(int value)](#setTextAlign-int-) | Represents how to align the text used by the control. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indicates whether the control is transparent. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indicates whether this control is visible. |
| [setWidth(double value)](#setWidth-double-) | Sets the width of the control in unit of points. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```
Gets the ole color of the background.
**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getData() {#getData--}
```
public byte[] getData()
```
Gets the binary data of the control.
**Returns:**
byte[]
### getFont() {#getFont--}
```
public Font getFont()
```
Represents the font of the control.
**Returns:**
[Font](../../com.aspose.cells/font)
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```
Gets the ole color of the foreground.
**Remarks**
Not applies to Image control.
**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```
Gets the height of the control in unit of points.
**Returns:**
double
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```
Gets the default run-time mode of the Input Method Editor for the control as it receives focus.
See [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).
**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```
Gets the linked cell.
**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```
Gets the list fill range.
**Returns:**
java.lang.String
### getMax() {#getMax--}
```
public int getMax()
```
Gets the maximum acceptable value.
**Example**
```
activeXControl.setMax(100);
```
**Returns:**
int
### getMin() {#getMin--}
```
public int getMin()
```
Gets the minimum acceptable value.
**Example**
```
activeXControl.setMin(0);
```
**Returns:**
int
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```
Gets a custom icon to display as the mouse pointer for the control.
**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```
Gets the type of icon displayed as the mouse pointer for the control.
See [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).
**Returns:**
int
### getOrientation() {#getOrientation--}
```
public int getOrientation()
```
Gets whether the SpinButton or ScrollBar is oriented vertically or horizontally.
See [ControlScrollOrientation](../../com.aspose.cells/controlscrollorientation).
**Example**
```
if(activeXControl.getOrientation() == com.aspose.cells.ControlScrollOrientation.AUTO)
{
activeXControl.setOrientation(com.aspose.cells.ControlScrollOrientation.HORIZONTAL);
}
```
**Returns:**
int
### getPosition() {#getPosition--}
```
public int getPosition()
```
Gets the value.
**Example**
```
activeXControl.setPosition(30);
```
**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```
Indicates whether to show a shadow.
**Returns:**
boolean
### getSmallChange() {#getSmallChange--}
```
public int getSmallChange()
```
Gets the amount by which the Position property changes
**Example**
```
activeXControl.setSmallChange(5);
```
**Returns:**
int
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```
Represents how to align the text used by the control.
See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).
**Returns:**
int
### getType() {#getType--}
```
public int getType()
```
Gets the type of the ActiveX control.
See [ControlType](../../com.aspose.cells/controltype).
**Example**
```
if(activeXControl.getType() == com.aspose.cells.ControlType.SPIN_BUTTON)
{
//do something
}
```
**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```
Gets the width of the control in unit of points.
**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```
Gets the [Workbook](../../com.aspose.cells/workbook) object.
**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isAutoSize() {#isAutoSize--}
```
public boolean isAutoSize()
```
Indicates whether the control will automatically resize to display its entire contents.
**Returns:**
boolean
### isEnabled() {#isEnabled--}
```
public boolean isEnabled()
```
Indicates whether the control can receive the focus and respond to user-generated events.
**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```
Indicates whether data in the control is locked for editing.
**Returns:**
boolean
### isTransparent() {#isTransparent--}
```
public boolean isTransparent()
```
Indicates whether the control is transparent.
**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```
Indicates whether this control is visible.
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
### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```
Indicates whether the control will automatically resize to display its entire contents.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```
Sets the ole color of the background.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```
Indicates whether the control can receive the focus and respond to user-generated events.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```
Sets the ole color of the foreground.
**Remarks**
Not applies to Image control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```
Sets the height of the control in unit of points.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```
Sets the default run-time mode of the Input Method Editor for the control as it receives focus.
See [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```
Sets the linked cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```
Sets the list fill range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```
Indicates whether data in the control is locked for editing.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setMax(int value) {#setMax-int-}
```
public void setMax(int value)
```
Sets the maximum acceptable value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setMin(int value) {#setMin-int-}
```
public void setMin(int value)
```
Sets the minimum acceptable value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```
Sets a custom icon to display as the mouse pointer for the control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |
### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```
Sets the type of icon displayed as the mouse pointer for the control.
See [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setOrientation(int value) {#setOrientation-int-}
```
public void setOrientation(int value)
```
Sets whether the SpinButton or ScrollBar is oriented vertically or horizontally.
See [ControlScrollOrientation](../../com.aspose.cells/controlscrollorientation).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```
Sets the value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```
Indicates whether to show a shadow.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSmallChange(int value) {#setSmallChange-int-}
```
public void setSmallChange(int value)
```
Sets the amount by which the Position property changes
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```
Represents how to align the text used by the control.
See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```
Indicates whether the control is transparent.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```
Indicates whether this control is visible.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```
Sets the width of the control in unit of points.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
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
