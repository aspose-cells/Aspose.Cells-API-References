##CheckBoxActiveXControl
Represents a CheckBox ActiveX control.
**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class CheckBoxActiveXControl extends ActiveXControl
```
Represents a CheckBox ActiveX control.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccelerator()](#getAccelerator--) | Gets the accelerator key for the control. |
| [getAlignment()](#getAlignment--) | Gets the position of the Caption relative to the control. |
| [getBackOleColor()](#getBackOleColor--) | Gets the ole color of the background. |
| [getCaption()](#getCaption--) | Gets the descriptive text that appears on a control. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Gets the binary data of the control. |
| [getFont()](#getFont--) | Represents the font of the control. |
| [getForeOleColor()](#getForeOleColor--) | Gets the ole color of the foreground. |
| [getGroupName()](#getGroupName--) | Gets the group's name. |
| [getHeight()](#getHeight--) | Gets the height of the control in unit of points. |
| [getIMEMode()](#getIMEMode--) | Gets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [getLinkedCell()](#getLinkedCell--) | Gets the linked cell. |
| [getListFillRange()](#getListFillRange--) | Gets the list fill range. |
| [getMouseIcon()](#getMouseIcon--) | Gets a custom icon to display as the mouse pointer for the control. |
| [getMousePointer()](#getMousePointer--) | Gets the type of icon displayed as the mouse pointer for the control. |
| [getPicture()](#getPicture--) | Gets the data of the picture. |
| [getPicturePosition()](#getPicturePosition--) | Gets the location of the control's picture relative to its caption. |
| [getShadow()](#getShadow--) | Indicates whether to show a shadow. |
| [getSpecialEffect()](#getSpecialEffect--) | Gets the special effect of the control. |
| [getTextAlign()](#getTextAlign--) | Represents how to align the text used by the control. |
| [getType()](#getType--) | Gets the type of the ActiveX control. |
| [getValue()](#getValue--) | Indicates if the control is checked or not. |
| [getWidth()](#getWidth--) | Gets the width of the control in unit of points. |
| [getWorkbook()](#getWorkbook--) | Gets the [Workbook](../../com.aspose.cells/workbook) object. |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Indicates whether the control will automatically resize to display its entire contents. |
| [isEnabled()](#isEnabled--) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [isLocked()](#isLocked--) | Indicates whether data in the control is locked for editing. |
| [isTransparent()](#isTransparent--) | Indicates whether the control is transparent. |
| [isTripleState()](#isTripleState--) | Indicates how the specified control will display Null values. |
| [isVisible()](#isVisible--) | Indicates whether this control is visible. |
| [isWordWrapped()](#isWordWrapped--) | Indicates whether the contents of the control automatically wrap at the end of a line. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccelerator(char value)](#setAccelerator-char-) | Sets the accelerator key for the control. |
| [setAlignment(int value)](#setAlignment-int-) | Sets the position of the Caption relative to the control. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indicates whether the control will automatically resize to display its entire contents. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Sets the ole color of the background. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Sets the descriptive text that appears on a control. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Sets the ole color of the foreground. |
| [setGroupName(String value)](#setGroupName-java.lang.String-) | Sets the group's name. |
| [setHeight(double value)](#setHeight-double-) | Sets the height of the control in unit of points. |
| [setIMEMode(int value)](#setIMEMode-int-) | Sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Sets the linked cell. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Sets the list fill range. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indicates whether data in the control is locked for editing. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Sets a custom icon to display as the mouse pointer for the control. |
| [setMousePointer(int value)](#setMousePointer-int-) | Sets the type of icon displayed as the mouse pointer for the control. |
| [setPicture(byte[] value)](#setPicture-byte---) | Sets the data of the picture. |
| [setPicturePosition(int value)](#setPicturePosition-int-) | Sets the location of the control's picture relative to its caption. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indicates whether to show a shadow. |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Sets the special effect of the control. |
| [setTextAlign(int value)](#setTextAlign-int-) | Represents how to align the text used by the control. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indicates whether the control is transparent. |
| [setTripleState(boolean value)](#setTripleState-boolean-) | Indicates how the specified control will display Null values. |
| [setValue(int value)](#setValue-int-) | Indicates if the control is checked or not. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indicates whether this control is visible. |
| [setWidth(double value)](#setWidth-double-) | Sets the width of the control in unit of points. |
| [setWordWrapped(boolean value)](#setWordWrapped-boolean-) | Indicates whether the contents of the control automatically wrap at the end of a line. |
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
### getAccelerator() {#getAccelerator--}
```
public char getAccelerator()
```
Gets the accelerator key for the control.
**Returns:**
char
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```
Gets the position of the Caption relative to the control.
See [ControlCaptionAlignmentType](../../com.aspose.cells/controlcaptionalignmenttype).
**Returns:**
int
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```
Gets the ole color of the background.
**Returns:**
int
### getCaption() {#getCaption--}
```
public String getCaption()
```
Gets the descriptive text that appears on a control.
**Returns:**
java.lang.String
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
### getGroupName() {#getGroupName--}
```
public String getGroupName()
```
Gets the group's name.
**Returns:**
java.lang.String
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
### getPicture() {#getPicture--}
```
public byte[] getPicture()
```
Gets the data of the picture.
**Returns:**
byte[]
### getPicturePosition() {#getPicturePosition--}
```
public int getPicturePosition()
```
Gets the location of the control's picture relative to its caption.
See [ControlPicturePositionType](../../com.aspose.cells/controlpicturepositiontype).
**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```
Indicates whether to show a shadow.
**Returns:**
boolean
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```
Gets the special effect of the control.
See [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).
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
**Returns:**
int
### getValue() {#getValue--}
```
public int getValue()
```
Indicates if the control is checked or not.
See [CheckValueType](../../com.aspose.cells/checkvaluetype).
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
### isTripleState() {#isTripleState--}
```
public boolean isTripleState()
```
Indicates how the specified control will display Null values.
**Remarks**
| Setting | Description                                                                                                                                     |
| ------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| True    | The control will cycle through states for Yes, No, and Null values. The control appears dimmed (grayed) when its Value property is set to Null. |
| False   | (Default) The control will cycle through states for Yes and No values. Null values display as if they were No values.                           |
**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```
Indicates whether this control is visible.
**Returns:**
boolean
### isWordWrapped() {#isWordWrapped--}
```
public boolean isWordWrapped()
```
Indicates whether the contents of the control automatically wrap at the end of a line.
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
### setAccelerator(char value) {#setAccelerator-char-}
```
public void setAccelerator(char value)
```
Sets the accelerator key for the control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```
Sets the position of the Caption relative to the control.
See [ControlCaptionAlignmentType](../../com.aspose.cells/controlcaptionalignmenttype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
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
### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```
Sets the descriptive text that appears on a control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
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
### setGroupName(String value) {#setGroupName-java.lang.String-}
```
public void setGroupName(String value)
```
Sets the group's name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
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
### setPicture(byte[] value) {#setPicture-byte---}
```
public void setPicture(byte[] value)
```
Sets the data of the picture.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |
### setPicturePosition(int value) {#setPicturePosition-int-}
```
public void setPicturePosition(int value)
```
Sets the location of the control's picture relative to its caption.
See [ControlPicturePositionType](../../com.aspose.cells/controlpicturepositiontype).
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
### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```
Sets the special effect of the control.
See [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).
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
### setTripleState(boolean value) {#setTripleState-boolean-}
```
public void setTripleState(boolean value)
```
Indicates how the specified control will display Null values.
**Remarks**
| Setting | Description                                                                                                                                     |
| ------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| True    | The control will cycle through states for Yes, No, and Null values. The control appears dimmed (grayed) when its Value property is set to Null. |
| False   | (Default) The control will cycle through states for Yes and No values. Null values display as if they were No values.                           |
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setValue(int value) {#setValue-int-}
```
public void setValue(int value)
```
Indicates if the control is checked or not.
See [CheckValueType](../../com.aspose.cells/checkvaluetype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
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
### setWordWrapped(boolean value) {#setWordWrapped-boolean-}
```
public void setWordWrapped(boolean value)
```
Indicates whether the contents of the control automatically wrap at the end of a line.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
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
