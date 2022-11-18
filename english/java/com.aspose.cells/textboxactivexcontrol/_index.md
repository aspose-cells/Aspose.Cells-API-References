---
title: TextBoxActiveXControl
second_title: Aspose.Cells for Java API Reference
description: Represents a text box ActiveX control.
type: docs
weight: 569
url: /java/com.aspose.cells/textboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class TextBoxActiveXControl extends ActiveXControl
```

Represents a text box ActiveX control.
## Constructors

| Constructor | Description |
| --- | --- |
| [TextBoxActiveXControl()](#TextBoxActiveXControl--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Gets and sets the ole color of the background. |
| [getBorderOleColor()](#getBorderOleColor--) | Gets and sets the ole color of the background. |
| [getBorderStyle()](#getBorderStyle--) | Gets and set the type of border used by the control. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Gets and sets the binary data of the control. |
| [getDropButtonStyle()](#getDropButtonStyle--) | Specifies the symbol displayed on the drop button |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | Specifies selection behavior when entering the control. |
| [getEnterKeyBehavior()](#getEnterKeyBehavior--) | Specifies the behavior of the ENTER key. |
| [getFont()](#getFont--) | Represents the font of the control. |
| [getForeOleColor()](#getForeOleColor--) | Gets and sets the ole color of the foreground. |
| [getHeight()](#getHeight--) | Gets and sets the height of the control in unit of points. |
| [getHideSelection()](#getHideSelection--) | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [getIMEMode()](#getIMEMode--) | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [getIntegralHeight()](#getIntegralHeight--) | Indicates whether the control will only show complete lines of text without showing any partial lines. |
| [getLinkedCell()](#getLinkedCell--) | Gets and sets the linked cell. |
| [getListFillRange()](#getListFillRange--) | Gets and sets the list fill range. |
| [getMaxLength()](#getMaxLength--) | Gets and sets the maximum number of characters |
| [getMouseIcon()](#getMouseIcon--) | Gets and sets a custom icon to display as the mouse pointer for the control. |
| [getMousePointer()](#getMousePointer--) | Gets and sets the type of icon displayed as the mouse pointer for the control. |
| [getPasswordChar()](#getPasswordChar--) | Gets and sets a character to be displayed in place of the characters entered. |
| [getScrollBars()](#getScrollBars--) | Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. |
| [getShadow()](#getShadow--) | Indicates whether to show a shadow. |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | Specifies the symbol displayed on the drop button |
| [getSpecialEffect()](#getSpecialEffect--) | Gets and sets the special effect of the control. |
| [getTabKeyBehavior()](#getTabKeyBehavior--) | Indicates whether tab characters are allowed in the text of the control. |
| [getText()](#getText--) | Gets and set text of the control. |
| [getTextAlign()](#getTextAlign--) | Represents how to align the text used by the control. |
| [getType()](#getType--) | Gets the type of the ActiveX control. |
| [getWidth()](#getWidth--) | Gets and sets the width of the control in unit of points. |
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
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | For the description of this property, please see \#isAutoSize().isAutoSize() |
| [setAutoTab(boolean value)](#setAutoTab-boolean-) | For the description of this property, please see \#isAutoTab().isAutoTab() |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) | For the description of this property, please see \#isAutoWordSelected().isAutoWordSelected() |
| [setBackOleColor(int value)](#setBackOleColor-int-) | For the description of this property, please see \#getBackOleColor().getBackOleColor() |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | For the description of this property, please see \#getBorderOleColor().getBorderOleColor() |
| [setBorderStyle(int value)](#setBorderStyle-int-) | For the description of this property, please see \#getBorderStyle().getBorderStyle() |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) | For the description of this property, please see \#isDragBehaviorEnabled().isDragBehaviorEnabled() |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) | For the description of this property, please see \#getDropButtonStyle().getDropButtonStyle() |
| [setEditable(boolean value)](#setEditable-boolean-) | For the description of this property, please see \#isEditable().isEditable() |
| [setEnabled(boolean value)](#setEnabled-boolean-) | For the description of this property, please see \#isEnabled().isEnabled() |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) | For the description of this property, please see \#getEnterFieldBehavior().getEnterFieldBehavior() |
| [setEnterKeyBehavior(boolean value)](#setEnterKeyBehavior-boolean-) | For the description of this property, please see \#getEnterKeyBehavior().getEnterKeyBehavior() |
| [setForeOleColor(int value)](#setForeOleColor-int-) | For the description of this property, please see \#getForeOleColor().getForeOleColor() |
| [setHeight(double value)](#setHeight-double-) | For the description of this property, please see \#getHeight().getHeight() |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) | For the description of this property, please see \#getHideSelection().getHideSelection() |
| [setIMEMode(int value)](#setIMEMode-int-) | For the description of this property, please see \#getIMEMode().getIMEMode() |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | For the description of this property, please see \#getIntegralHeight().getIntegralHeight() |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | For the description of this property, please see \#getLinkedCell().getLinkedCell() |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | For the description of this property, please see \#getListFillRange().getListFillRange() |
| [setLocked(boolean value)](#setLocked-boolean-) | For the description of this property, please see \#isLocked().isLocked() |
| [setMaxLength(int value)](#setMaxLength-int-) | For the description of this property, please see \#getMaxLength().getMaxLength() |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | For the description of this property, please see \#getMouseIcon().getMouseIcon() |
| [setMousePointer(int value)](#setMousePointer-int-) | For the description of this property, please see \#getMousePointer().getMousePointer() |
| [setMultiLine(boolean value)](#setMultiLine-boolean-) | For the description of this property, please see \#isMultiLine().isMultiLine() |
| [setPasswordChar(char value)](#setPasswordChar-char-) | For the description of this property, please see \#getPasswordChar().getPasswordChar() |
| [setScrollBars(int value)](#setScrollBars-int-) | For the description of this property, please see \#getScrollBars().getScrollBars() |
| [setShadow(boolean value)](#setShadow-boolean-) | For the description of this property, please see \#getShadow().getShadow() |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) | For the description of this property, please see \#getShowDropButtonTypeWhen().getShowDropButtonTypeWhen() |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | For the description of this property, please see \#getSpecialEffect().getSpecialEffect() |
| [setTabKeyBehavior(boolean value)](#setTabKeyBehavior-boolean-) | For the description of this property, please see \#getTabKeyBehavior().getTabKeyBehavior() |
| [setText(String value)](#setText-java.lang.String-) | For the description of this property, please see \#getText().getText() |
| [setTextAlign(int value)](#setTextAlign-int-) | For the description of this property, please see \#getTextAlign().getTextAlign() |
| [setTransparent(boolean value)](#setTransparent-boolean-) | For the description of this property, please see \#isTransparent().isTransparent() |
| [setVisible(boolean value)](#setVisible-boolean-) | For the description of this property, please see \#isVisible().isVisible() |
| [setWidth(double value)](#setWidth-double-) | For the description of this property, please see \#getWidth().getWidth() |
| [setWordWrapped(boolean value)](#setWordWrapped-boolean-) | For the description of this property, please see \#isWordWrapped().isWordWrapped() |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TextBoxActiveXControl() {#TextBoxActiveXControl--}
```
public TextBoxActiveXControl()
```


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


Gets and sets the ole color of the background.

**Returns:**
int
### getBorderOleColor() {#getBorderOleColor--}
```
public int getBorderOleColor()
```


Gets and sets the ole color of the background.

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Gets and set the type of border used by the control.

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


Gets and sets the binary data of the control.

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


Gets and sets the ole color of the foreground. Not applies to Image control.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Gets and sets the height of the control in unit of points.

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


Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus.

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


Gets and sets the linked cell.

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


Gets and sets the list fill range.

**Returns:**
java.lang.String
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Gets and sets the maximum number of characters

**Returns:**
int
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


Gets and sets a custom icon to display as the mouse pointer for the control.

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


Gets and sets the type of icon displayed as the mouse pointer for the control.

**Returns:**
int
### getPasswordChar() {#getPasswordChar--}
```
public char getPasswordChar()
```


Gets and sets a character to be displayed in place of the characters entered.

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


Gets and sets the special effect of the control.

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


Gets and set text of the control.

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


Gets and sets the width of the control in unit of points.

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


For the description of this property, please see \#isAutoSize().isAutoSize()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoTab(boolean value) {#setAutoTab-boolean-}
```
public void setAutoTab(boolean value)
```


For the description of this property, please see \#isAutoTab().isAutoTab()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoWordSelected(boolean value) {#setAutoWordSelected-boolean-}
```
public void setAutoWordSelected(boolean value)
```


For the description of this property, please see \#isAutoWordSelected().isAutoWordSelected()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


For the description of this property, please see \#getBackOleColor().getBackOleColor()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBorderOleColor(int value) {#setBorderOleColor-int-}
```
public void setBorderOleColor(int value)
```


For the description of this property, please see \#getBorderOleColor().getBorderOleColor()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


For the description of this property, please see \#getBorderStyle().getBorderStyle()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDragBehaviorEnabled(boolean value) {#setDragBehaviorEnabled-boolean-}
```
public void setDragBehaviorEnabled(boolean value)
```


For the description of this property, please see \#isDragBehaviorEnabled().isDragBehaviorEnabled()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDropButtonStyle(int value) {#setDropButtonStyle-int-}
```
public void setDropButtonStyle(int value)
```


For the description of this property, please see \#getDropButtonStyle().getDropButtonStyle()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setEditable(boolean value) {#setEditable-boolean-}
```
public void setEditable(boolean value)
```


For the description of this property, please see \#isEditable().isEditable()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


For the description of this property, please see \#isEnabled().isEnabled()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnterFieldBehavior(boolean value) {#setEnterFieldBehavior-boolean-}
```
public void setEnterFieldBehavior(boolean value)
```


For the description of this property, please see \#getEnterFieldBehavior().getEnterFieldBehavior()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnterKeyBehavior(boolean value) {#setEnterKeyBehavior-boolean-}
```
public void setEnterKeyBehavior(boolean value)
```


For the description of this property, please see \#getEnterKeyBehavior().getEnterKeyBehavior()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


For the description of this property, please see \#getForeOleColor().getForeOleColor()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


For the description of this property, please see \#getHeight().getHeight()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHideSelection(boolean value) {#setHideSelection-boolean-}
```
public void setHideSelection(boolean value)
```


For the description of this property, please see \#getHideSelection().getHideSelection()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


For the description of this property, please see \#getIMEMode().getIMEMode()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setIntegralHeight(boolean value) {#setIntegralHeight-boolean-}
```
public void setIntegralHeight(boolean value)
```


For the description of this property, please see \#getIntegralHeight().getIntegralHeight()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


For the description of this property, please see \#getLinkedCell().getLinkedCell()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


For the description of this property, please see \#getListFillRange().getListFillRange()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


For the description of this property, please see \#isLocked().isLocked()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


For the description of this property, please see \#getMaxLength().getMaxLength()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


For the description of this property, please see \#getMouseIcon().getMouseIcon()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


For the description of this property, please see \#getMousePointer().getMousePointer()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMultiLine(boolean value) {#setMultiLine-boolean-}
```
public void setMultiLine(boolean value)
```


For the description of this property, please see \#isMultiLine().isMultiLine()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPasswordChar(char value) {#setPasswordChar-char-}
```
public void setPasswordChar(char value)
```


For the description of this property, please see \#getPasswordChar().getPasswordChar()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |

### setScrollBars(int value) {#setScrollBars-int-}
```
public void setScrollBars(int value)
```


For the description of this property, please see \#getScrollBars().getScrollBars()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


For the description of this property, please see \#getShadow().getShadow()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowDropButtonTypeWhen(int value) {#setShowDropButtonTypeWhen-int-}
```
public void setShowDropButtonTypeWhen(int value)
```


For the description of this property, please see \#getShowDropButtonTypeWhen().getShowDropButtonTypeWhen()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```


For the description of this property, please see \#getSpecialEffect().getSpecialEffect()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTabKeyBehavior(boolean value) {#setTabKeyBehavior-boolean-}
```
public void setTabKeyBehavior(boolean value)
```


For the description of this property, please see \#getTabKeyBehavior().getTabKeyBehavior()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


For the description of this property, please see \#getText().getText()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


For the description of this property, please see \#getTextAlign().getTextAlign()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


For the description of this property, please see \#isTransparent().isTransparent()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


For the description of this property, please see \#isVisible().isVisible()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


For the description of this property, please see \#getWidth().getWidth()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWordWrapped(boolean value) {#setWordWrapped-boolean-}
```
public void setWordWrapped(boolean value)
```


For the description of this property, please see \#isWordWrapped().isWordWrapped()

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

