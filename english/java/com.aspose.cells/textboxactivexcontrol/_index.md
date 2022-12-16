---
title: TextBoxActiveXControl
second_title: Aspose.Cells for Java API Reference
description: Represents a text box ActiveX control.
type: docs
url: /java/com.aspose.cells/textboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class TextBoxActiveXControl extends ActiveXControl
```

Represents a text box ActiveX control.
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Gets the ole color of the background. |
| [getBorderOleColor()](#getBorderOleColor--) | Gets the ole color of the background. |
| [getBorderStyle()](#getBorderStyle--) | Gets the type of border used by the control. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Gets the binary data of the control. |
| [getDropButtonStyle()](#getDropButtonStyle--) | Specifies the symbol displayed on the drop button |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | Specifies selection behavior when entering the control. |
| [getEnterKeyBehavior()](#getEnterKeyBehavior--) | Specifies the behavior of the ENTER key. |
| [getFont()](#getFont--) | Represents the font of the control. |
| [getForeOleColor()](#getForeOleColor--) | Gets the ole color of the foreground. |
| [getHeight()](#getHeight--) | Gets the height of the control in unit of points. |
| [getHideSelection()](#getHideSelection--) | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [getIMEMode()](#getIMEMode--) | Gets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [getIntegralHeight()](#getIntegralHeight--) | Indicates whether the control will only show complete lines of text without showing any partial lines. |
| [getLinkedCell()](#getLinkedCell--) | Gets the linked cell. |
| [getListFillRange()](#getListFillRange--) | Gets the list fill range. |
| [getMaxLength()](#getMaxLength--) | Gets the maximum number of characters |
| [getMouseIcon()](#getMouseIcon--) | Gets a custom icon to display as the mouse pointer for the control. |
| [getMousePointer()](#getMousePointer--) | Gets the type of icon displayed as the mouse pointer for the control. |
| [getPasswordChar()](#getPasswordChar--) | Gets a character to be displayed in place of the characters entered. |
| [getScrollBars()](#getScrollBars--) | Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. |
| [getShadow()](#getShadow--) | Indicates whether to show a shadow. |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | Specifies the symbol displayed on the drop button |
| [getSpecialEffect()](#getSpecialEffect--) | Gets the special effect of the control. |
| [getTabKeyBehavior()](#getTabKeyBehavior--) | Indicates whether tab characters are allowed in the text of the control. |
| [getText()](#getText--) | Gets text of the control. |
| [getTextAlign()](#getTextAlign--) | Represents how to align the text used by the control. |
| [getType()](#getType--) | Gets the type of the ActiveX control. |
| [getWidth()](#getWidth--) | Gets the width of the control in unit of points. |
| [getWorkbook()](#getWorkbook--) | Gets the [Workbook](../../com.aspose.cells/workbook) object. |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Indicates whether the control will automatically resize to display its entire contents. |
| [isAutoTab()](#isAutoTab--) | Indicates whether the focus will automatically move to the next control when the user enters the maximum number of characters. |
| [isAutoWordSelected()](#isAutoWordSelected--) | Specifies the basic unit used to extend a selection. |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--) | Indicates whether dragging and dropping is enabled for the control. |
| [isEditable()](#isEditable--) | Indicates whether the user can type into the control. |
| [isEnabled()](#isEnabled--) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [isLocked()](#isLocked--) | Indicates whether data in the control is locked for editing. |
| [isMultiLine()](#isMultiLine--) | Indicates whether the control can display more than one line of text. |
| [isTransparent()](#isTransparent--) | Indicates whether the control is transparent. |
| [isVisible()](#isVisible--) | Indicates whether this control is visible. |
| [isWordWrapped()](#isWordWrapped--) | Indicates whether the contents of the control automatically wrap at the end of a line. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indicates whether the control will automatically resize to display its entire contents. |
| [setAutoTab(boolean value)](#setAutoTab-boolean-) | Indicates whether the focus will automatically move to the next control when the user enters the maximum number of characters. |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) | Specifies the basic unit used to extend a selection. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Sets the ole color of the background. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Sets the ole color of the background. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Sets the type of border used by the control. |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) | Indicates whether dragging and dropping is enabled for the control. |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) | Specifies the symbol displayed on the drop button |
| [setEditable(boolean value)](#setEditable-boolean-) | Indicates whether the user can type into the control. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) | Specifies selection behavior when entering the control. |
| [setEnterKeyBehavior(boolean value)](#setEnterKeyBehavior-boolean-) | Specifies the behavior of the ENTER key. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Sets the ole color of the foreground. |
| [setHeight(double value)](#setHeight-double-) | Sets the height of the control in unit of points. |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [setIMEMode(int value)](#setIMEMode-int-) | Sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | Indicates whether the control will only show complete lines of text without showing any partial lines. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Sets the linked cell. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Sets the list fill range. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indicates whether data in the control is locked for editing. |
| [setMaxLength(int value)](#setMaxLength-int-) | Sets the maximum number of characters |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Sets a custom icon to display as the mouse pointer for the control. |
| [setMousePointer(int value)](#setMousePointer-int-) | Sets the type of icon displayed as the mouse pointer for the control. |
| [setMultiLine(boolean value)](#setMultiLine-boolean-) | Indicates whether the control can display more than one line of text. |
| [setPasswordChar(char value)](#setPasswordChar-char-) | Sets a character to be displayed in place of the characters entered. |
| [setScrollBars(int value)](#setScrollBars-int-) | Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indicates whether to show a shadow. |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) | Specifies the symbol displayed on the drop button |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Sets the special effect of the control. |
| [setTabKeyBehavior(boolean value)](#setTabKeyBehavior-boolean-) | Indicates whether tab characters are allowed in the text of the control. |
| [setText(String value)](#setText-java.lang.String-) | Sets text of the control. |
| [setTextAlign(int value)](#setTextAlign-int-) | Represents how to align the text used by the control. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indicates whether the control is transparent. |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Gets the ole color of the background.

**Returns:**
int
### getBorderOleColor() {#getBorderOleColor--}
```
public int getBorderOleColor()
```


Gets the ole color of the background.

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Gets the type of border used by the control.

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
### getDropButtonStyle() {#getDropButtonStyle--}
```
public int getDropButtonStyle()
```


Specifies the symbol displayed on the drop button

**Returns:**
int
### getEnterFieldBehavior() {#getEnterFieldBehavior--}
```
public boolean getEnterFieldBehavior()
```


Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control.

**Returns:**
boolean
### getEnterKeyBehavior() {#getEnterKeyBehavior--}
```
public boolean getEnterKeyBehavior()
```


Specifies the behavior of the ENTER key. True specifies that pressing ENTER will create a new line. False specifies that pressing ENTER will move the focus to the next object in the tab order.

**Returns:**
boolean
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


Gets the ole color of the foreground. Not applies to Image control.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Gets the height of the control in unit of points.

**Returns:**
double
### getHideSelection() {#getHideSelection--}
```
public boolean getHideSelection()
```


Indicates whether selected text in the control appears highlighted when the control does not have focus.

**Returns:**
boolean
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```


Gets the default run-time mode of the Input Method Editor for the control as it receives focus.

**Returns:**
int
### getIntegralHeight() {#getIntegralHeight--}
```
public boolean getIntegralHeight()
```


Indicates whether the control will only show complete lines of text without showing any partial lines.

**Returns:**
boolean
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
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Gets the maximum number of characters

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

**Returns:**
int
### getPasswordChar() {#getPasswordChar--}
```
public char getPasswordChar()
```


Gets a character to be displayed in place of the characters entered.

**Returns:**
char
### getScrollBars() {#getScrollBars--}
```
public int getScrollBars()
```


Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither.

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Indicates whether to show a shadow.

**Returns:**
boolean
### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}
```
public int getShowDropButtonTypeWhen()
```


Specifies the symbol displayed on the drop button

**Returns:**
int
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


Gets the special effect of the control.

**Returns:**
int
### getTabKeyBehavior() {#getTabKeyBehavior--}
```
public boolean getTabKeyBehavior()
```


Indicates whether tab characters are allowed in the text of the control.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Gets text of the control.

**Returns:**
java.lang.String
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


Represents how to align the text used by the control.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Gets the type of the ActiveX control.

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
### isAutoTab() {#isAutoTab--}
```
public boolean isAutoTab()
```


Indicates whether the focus will automatically move to the next control when the user enters the maximum number of characters.

**Returns:**
boolean
### isAutoWordSelected() {#isAutoWordSelected--}
```
public boolean isAutoWordSelected()
```


Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false specifies that the basic unit is a whole word.

**Returns:**
boolean
### isDragBehaviorEnabled() {#isDragBehaviorEnabled--}
```
public boolean isDragBehaviorEnabled()
```


Indicates whether dragging and dropping is enabled for the control.

**Returns:**
boolean
### isEditable() {#isEditable--}
```
public boolean isEditable()
```


Indicates whether the user can type into the control.

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
### isMultiLine() {#isMultiLine--}
```
public boolean isMultiLine()
```


Indicates whether the control can display more than one line of text.

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




### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Indicates whether the control will automatically resize to display its entire contents.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoTab(boolean value) {#setAutoTab-boolean-}
```
public void setAutoTab(boolean value)
```


Indicates whether the focus will automatically move to the next control when the user enters the maximum number of characters.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoWordSelected(boolean value) {#setAutoWordSelected-boolean-}
```
public void setAutoWordSelected(boolean value)
```


Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false specifies that the basic unit is a whole word.

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

### setBorderOleColor(int value) {#setBorderOleColor-int-}
```
public void setBorderOleColor(int value)
```


Sets the ole color of the background.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Sets the type of border used by the control.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDragBehaviorEnabled(boolean value) {#setDragBehaviorEnabled-boolean-}
```
public void setDragBehaviorEnabled(boolean value)
```


Indicates whether dragging and dropping is enabled for the control.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDropButtonStyle(int value) {#setDropButtonStyle-int-}
```
public void setDropButtonStyle(int value)
```


Specifies the symbol displayed on the drop button

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setEditable(boolean value) {#setEditable-boolean-}
```
public void setEditable(boolean value)
```


Indicates whether the user can type into the control.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Indicates whether the control can receive the focus and respond to user-generated events.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnterFieldBehavior(boolean value) {#setEnterFieldBehavior-boolean-}
```
public void setEnterFieldBehavior(boolean value)
```


Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnterKeyBehavior(boolean value) {#setEnterKeyBehavior-boolean-}
```
public void setEnterKeyBehavior(boolean value)
```


Specifies the behavior of the ENTER key. True specifies that pressing ENTER will create a new line. False specifies that pressing ENTER will move the focus to the next object in the tab order.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


Sets the ole color of the foreground. Not applies to Image control.

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

### setHideSelection(boolean value) {#setHideSelection-boolean-}
```
public void setHideSelection(boolean value)
```


Indicates whether selected text in the control appears highlighted when the control does not have focus.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


Sets the default run-time mode of the Input Method Editor for the control as it receives focus.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setIntegralHeight(boolean value) {#setIntegralHeight-boolean-}
```
public void setIntegralHeight(boolean value)
```


Indicates whether the control will only show complete lines of text without showing any partial lines.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


Sets the maximum number of characters

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

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMultiLine(boolean value) {#setMultiLine-boolean-}
```
public void setMultiLine(boolean value)
```


Indicates whether the control can display more than one line of text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPasswordChar(char value) {#setPasswordChar-char-}
```
public void setPasswordChar(char value)
```


Sets a character to be displayed in place of the characters entered.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |

### setScrollBars(int value) {#setScrollBars-int-}
```
public void setScrollBars(int value)
```


Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither.

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

### setShowDropButtonTypeWhen(int value) {#setShowDropButtonTypeWhen-int-}
```
public void setShowDropButtonTypeWhen(int value)
```


Specifies the symbol displayed on the drop button

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```


Sets the special effect of the control.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTabKeyBehavior(boolean value) {#setTabKeyBehavior-boolean-}
```
public void setTabKeyBehavior(boolean value)
```


Indicates whether tab characters are allowed in the text of the control.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Sets text of the control.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


Represents how to align the text used by the control.

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

