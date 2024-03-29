---
title: ListBoxActiveXControl
second_title: Aspose.Cells for Java API Reference
description: Represents a ListBox ActiveX control.
type: docs
url: /java/com.aspose.cells/listboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class ListBoxActiveXControl extends ActiveXControl
```

Represents a ListBox ActiveX control.
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Gets the ole color of the background. |
| [getBorderOleColor()](#getBorderOleColor--) | Gets the ole color of the background. |
| [getBorderStyle()](#getBorderStyle--) | Gets the type of border used by the control. |
| [getBoundColumn()](#getBoundColumn--) | Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle). |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Represents the number of columns to display in a ComboBox or ListBox. |
| [getColumnWidths()](#getColumnWidths--) | Gets the width of the column. |
| [getData()](#getData--) | Gets the binary data of the control. |
| [getFont()](#getFont--) | Represents the font of the control. |
| [getForeOleColor()](#getForeOleColor--) | Gets the ole color of the foreground. |
| [getHeight()](#getHeight--) | Gets the height of the control in unit of points. |
| [getIMEMode()](#getIMEMode--) | Gets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [getIntegralHeight()](#getIntegralHeight--) | Indicates whether the control will only show complete lines of text without showing any partial lines. |
| [getLinkedCell()](#getLinkedCell--) | Gets the linked cell. |
| [getListFillRange()](#getListFillRange--) | Gets the list fill range. |
| [getListStyle()](#getListStyle--) | Gets the visual appearance. |
| [getListWidth()](#getListWidth--) | Gets the width in unit of points. |
| [getMatchEntry()](#getMatchEntry--) | Indicates how a ListBox or ComboBox searches its list as the user types. |
| [getMouseIcon()](#getMouseIcon--) | Gets a custom icon to display as the mouse pointer for the control. |
| [getMousePointer()](#getMousePointer--) | Gets the type of icon displayed as the mouse pointer for the control. |
| [getScrollBars()](#getScrollBars--) | Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. |
| [getSelectionType()](#getSelectionType--) | Indicates whether the control permits multiple selections. |
| [getShadow()](#getShadow--) | Indicates whether to show a shadow. |
| [getShowColumnHeads()](#getShowColumnHeads--) | Indicates whether column headings are displayed. |
| [getSpecialEffect()](#getSpecialEffect--) | Gets the special effect of the control. |
| [getTextAlign()](#getTextAlign--) | Represents how to align the text used by the control. |
| [getTextColumn()](#getTextColumn--) | Represents the column in a ComboBox or ListBox to display to the user. |
| [getType()](#getType--) | Gets the type of the ActiveX control. |
| [getValue()](#getValue--) | Gets the value of the control. |
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
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Sets the ole color of the background. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Sets the type of border used by the control. |
| [setBoundColumn(int value)](#setBoundColumn-int-) | Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle). |
| [setColumnCount(int value)](#setColumnCount-int-) | Represents the number of columns to display in a ComboBox or ListBox. |
| [setColumnWidths(double value)](#setColumnWidths-double-) | Sets the width of the column. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Sets the ole color of the foreground. |
| [setHeight(double value)](#setHeight-double-) | Sets the height of the control in unit of points. |
| [setIMEMode(int value)](#setIMEMode-int-) | Sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | Indicates whether the control will only show complete lines of text without showing any partial lines. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Sets the linked cell. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Sets the list fill range. |
| [setListStyle(int value)](#setListStyle-int-) | Sets the visual appearance. |
| [setListWidth(double value)](#setListWidth-double-) | Sets the width in unit of points. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indicates whether data in the control is locked for editing. |
| [setMatchEntry(int value)](#setMatchEntry-int-) | Indicates how a ListBox or ComboBox searches its list as the user types. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Sets a custom icon to display as the mouse pointer for the control. |
| [setMousePointer(int value)](#setMousePointer-int-) | Sets the type of icon displayed as the mouse pointer for the control. |
| [setScrollBars(int value)](#setScrollBars-int-) | Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. |
| [setSelectionType(int value)](#setSelectionType-int-) | Indicates whether the control permits multiple selections. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indicates whether to show a shadow. |
| [setShowColumnHeads(boolean value)](#setShowColumnHeads-boolean-) | Indicates whether column headings are displayed. |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Sets the special effect of the control. |
| [setTextAlign(int value)](#setTextAlign-int-) | Represents how to align the text used by the control. |
| [setTextColumn(int value)](#setTextColumn-int-) | Represents the column in a ComboBox or ListBox to display to the user. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indicates whether the control is transparent. |
| [setValue(String value)](#setValue-java.lang.String-) | Sets the value of the control. |
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

See [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Returns:**
int
### getBoundColumn() {#getBoundColumn--}
```
public int getBoundColumn()
```


Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Represents the number of columns to display in a ComboBox or ListBox.

**Returns:**
int
### getColumnWidths() {#getColumnWidths--}
```
public double getColumnWidths()
```


Gets the width of the column.

**Returns:**
double
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
### getListStyle() {#getListStyle--}
```
public int getListStyle()
```


Gets the visual appearance.

See [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Returns:**
int
### getListWidth() {#getListWidth--}
```
public double getListWidth()
```


Gets the width in unit of points.

**Returns:**
double
### getMatchEntry() {#getMatchEntry--}
```
public int getMatchEntry()
```


Indicates how a ListBox or ComboBox searches its list as the user types.

See [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

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
### getScrollBars() {#getScrollBars--}
```
public int getScrollBars()
```


Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither.

See [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Returns:**
int
### getSelectionType() {#getSelectionType--}
```
public int getSelectionType()
```


Indicates whether the control permits multiple selections.

See [SelectionType](../../com.aspose.cells/selectiontype).

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Indicates whether to show a shadow.

**Returns:**
boolean
### getShowColumnHeads() {#getShowColumnHeads--}
```
public boolean getShowColumnHeads()
```


Indicates whether column headings are displayed.

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
### getTextColumn() {#getTextColumn--}
```
public int getTextColumn()
```


Represents the column in a ComboBox or ListBox to display to the user.

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
public String getValue()
```


Gets the value of the control.

**Remarks**

Only effects when [getSelectionType()](../../com.aspose.cells/listboxactivexcontrol\#getSelectionType--) is SelectionType.Single;

**Returns:**
java.lang.String
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

See [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBoundColumn(int value) {#setBoundColumn-int-}
```
public void setBoundColumn(int value)
```


Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setColumnCount(int value) {#setColumnCount-int-}
```
public void setColumnCount(int value)
```


Represents the number of columns to display in a ComboBox or ListBox.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setColumnWidths(double value) {#setColumnWidths-double-}
```
public void setColumnWidths(double value)
```


Sets the width of the column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

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

### setListStyle(int value) {#setListStyle-int-}
```
public void setListStyle(int value)
```


Sets the visual appearance.

See [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setListWidth(double value) {#setListWidth-double-}
```
public void setListWidth(double value)
```


Sets the width in unit of points.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Indicates whether data in the control is locked for editing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMatchEntry(int value) {#setMatchEntry-int-}
```
public void setMatchEntry(int value)
```


Indicates how a ListBox or ComboBox searches its list as the user types.

See [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

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

### setScrollBars(int value) {#setScrollBars-int-}
```
public void setScrollBars(int value)
```


Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither.

See [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSelectionType(int value) {#setSelectionType-int-}
```
public void setSelectionType(int value)
```


Indicates whether the control permits multiple selections.

See [SelectionType](../../com.aspose.cells/selectiontype).

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

### setShowColumnHeads(boolean value) {#setShowColumnHeads-boolean-}
```
public void setShowColumnHeads(boolean value)
```


Indicates whether column headings are displayed.

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

### setTextColumn(int value) {#setTextColumn-int-}
```
public void setTextColumn(int value)
```


Represents the column in a ComboBox or ListBox to display to the user.

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

### setValue(String value) {#setValue-java.lang.String-}
```
public void setValue(String value)
```


Sets the value of the control.

**Remarks**

Only effects when [getSelectionType()](../../com.aspose.cells/listboxactivexcontrol\#getSelectionType--) is SelectionType.Single;

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

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

