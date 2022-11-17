---
title: ComboBoxActiveXControl
second_title: Aspose.Cells for Java API Reference
description: Represents a ComboBox ActiveX control.
type: docs
weight: 100
url: /java/com.aspose.cells/comboboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class ComboBoxActiveXControl extends ActiveXControl
```

Represents a ComboBox ActiveX control.
## Constructors

| Constructor | Description |
| --- | --- |
| [ComboBoxActiveXControl()](#ComboBoxActiveXControl--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Gets and sets the ole color of the background. |
| [getBorderOleColor()](#getBorderOleColor--) | Gets and sets the ole color of the background. |
| [getBorderStyle()](#getBorderStyle--) | Gets and set the type of border used by the control. |
| [getBoundColumn()](#getBoundColumn--) | Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle). |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Represents the number of columns to display in a ComboBox or ListBox. |
| [getColumnWidths()](#getColumnWidths--) | Gets and sets the width of the column. |
| [getData()](#getData--) | Gets and sets the binary data of the control. |
| [getDropButtonStyle()](#getDropButtonStyle--) | Specifies the symbol displayed on the drop button |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | Specifies selection behavior when entering the control. |
| [getFont()](#getFont--) | Represents the font of the control. |
| [getForeOleColor()](#getForeOleColor--) | Gets and sets the ole color of the foreground. |
| [getHeight()](#getHeight--) | Gets and sets the height of the control in unit of points. |
| [getHideSelection()](#getHideSelection--) | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [getIMEMode()](#getIMEMode--) | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [getLinkedCell()](#getLinkedCell--) | Gets and sets the linked cell. |
| [getListFillRange()](#getListFillRange--) | Gets and sets the list fill range. |
| [getListRows()](#getListRows--) | Represents the maximum number of rows to display in the list. |
| [getListStyle()](#getListStyle--) | Gets and sets the visual appearance. |
| [getListWidth()](#getListWidth--) | Gets and set the width in unit of points. |
| [getMatchEntry()](#getMatchEntry--) | Indicates how a ListBox or ComboBox searches its list as the user types. |
| [getMaxLength()](#getMaxLength--) | Gets and sets the maximum number of characters |
| [getMouseIcon()](#getMouseIcon--) | Gets and sets a custom icon to display as the mouse pointer for the control. |
| [getMousePointer()](#getMousePointer--) | Gets and sets the type of icon displayed as the mouse pointer for the control. |
| [getSelectionMargin()](#getSelectionMargin--) | Indicates whether the user can select a line of text by clicking in the region to the left of the text. |
| [getShadow()](#getShadow--) | Indicates whether to show a shadow. |
| [getShowColumnHeads()](#getShowColumnHeads--) | Indicates whether column headings are displayed. |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | Specifies the symbol displayed on the drop button |
| [getSpecialEffect()](#getSpecialEffect--) | Gets and sets the special effect of the control. |
| [getTextAlign()](#getTextAlign--) | Represents how to align the text used by the control. |
| [getTextColumn()](#getTextColumn--) | Represents the column in a ComboBox or ListBox to display to the user. |
| [getType()](#getType--) | Gets the type of the ActiveX control. |
| [getValue()](#getValue--) | Gets and sets the value of the control. |
| [getWidth()](#getWidth--) | Gets and sets the width of the control in unit of points. |
| [getWorkbook()](#getWorkbook--) | Gets the [Workbook](../../com.aspose.cells/workbook) object. |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Indicates whether the control will automatically resize to display its entire contents. |
| [isAutoWordSelected()](#isAutoWordSelected--) | Specifies the basic unit used to extend a selection. |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--) | Indicates whether dragging and dropping is enabled for the control. |
| [isEditable()](#isEditable--) | Indicates whether the user can type into the control. |
| [isEnabled()](#isEnabled--) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [isLocked()](#isLocked--) | Indicates whether data in the control is locked for editing. |
| [isTransparent()](#isTransparent--) | Indicates whether the control is transparent. |
| [isVisible()](#isVisible--) | Indicates whether this control is visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) |  |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) |  |
| [setBackOleColor(int value)](#setBackOleColor-int-) |  |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) |  |
| [setBorderStyle(int value)](#setBorderStyle-int-) |  |
| [setBoundColumn(int value)](#setBoundColumn-int-) |  |
| [setColumnCount(int value)](#setColumnCount-int-) |  |
| [setColumnWidths(double value)](#setColumnWidths-double-) |  |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) |  |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) |  |
| [setEditable(boolean value)](#setEditable-boolean-) |  |
| [setEnabled(boolean value)](#setEnabled-boolean-) |  |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) |  |
| [setForeOleColor(int value)](#setForeOleColor-int-) |  |
| [setHeight(double value)](#setHeight-double-) |  |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) |  |
| [setIMEMode(int value)](#setIMEMode-int-) |  |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) |  |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) |  |
| [setListRows(int value)](#setListRows-int-) |  |
| [setListStyle(int value)](#setListStyle-int-) |  |
| [setListWidth(double value)](#setListWidth-double-) |  |
| [setLocked(boolean value)](#setLocked-boolean-) |  |
| [setMatchEntry(int value)](#setMatchEntry-int-) |  |
| [setMaxLength(int value)](#setMaxLength-int-) |  |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) |  |
| [setMousePointer(int value)](#setMousePointer-int-) |  |
| [setSelectionMargin(boolean value)](#setSelectionMargin-boolean-) |  |
| [setShadow(boolean value)](#setShadow-boolean-) |  |
| [setShowColumnHeads(boolean value)](#setShowColumnHeads-boolean-) |  |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) |  |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) |  |
| [setTextAlign(int value)](#setTextAlign-int-) |  |
| [setTextColumn(int value)](#setTextColumn-int-) |  |
| [setTransparent(boolean value)](#setTransparent-boolean-) |  |
| [setValue(String value)](#setValue-java.lang.String-) |  |
| [setVisible(boolean value)](#setVisible-boolean-) |  |
| [setWidth(double value)](#setWidth-double-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ComboBoxActiveXControl() {#ComboBoxActiveXControl--}
```
public ComboBoxActiveXControl()
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


Gets and sets the width of the column.

**Returns:**
double
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
### getListRows() {#getListRows--}
```
public int getListRows()
```


Represents the maximum number of rows to display in the list.

**Returns:**
int
### getListStyle() {#getListStyle--}
```
public int getListStyle()
```


Gets and sets the visual appearance.

**Returns:**
int
### getListWidth() {#getListWidth--}
```
public double getListWidth()
```


Gets and set the width in unit of points.

**Returns:**
double
### getMatchEntry() {#getMatchEntry--}
```
public int getMatchEntry()
```


Indicates how a ListBox or ComboBox searches its list as the user types.

**Returns:**
int
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
### getSelectionMargin() {#getSelectionMargin--}
```
public boolean getSelectionMargin()
```


Indicates whether the user can select a line of text by clicking in the region to the left of the text.

**Returns:**
boolean
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
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


Represents how to align the text used by the control.

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

**Returns:**
int
### getValue() {#getValue--}
```
public String getValue()
```


Gets and sets the value of the control.

**Returns:**
java.lang.String
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




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoWordSelected(boolean value) {#setAutoWordSelected-boolean-}
```
public void setAutoWordSelected(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBorderOleColor(int value) {#setBorderOleColor-int-}
```
public void setBorderOleColor(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBoundColumn(int value) {#setBoundColumn-int-}
```
public void setBoundColumn(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setColumnCount(int value) {#setColumnCount-int-}
```
public void setColumnCount(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setColumnWidths(double value) {#setColumnWidths-double-}
```
public void setColumnWidths(double value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setDragBehaviorEnabled(boolean value) {#setDragBehaviorEnabled-boolean-}
```
public void setDragBehaviorEnabled(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDropButtonStyle(int value) {#setDropButtonStyle-int-}
```
public void setDropButtonStyle(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setEditable(boolean value) {#setEditable-boolean-}
```
public void setEditable(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnterFieldBehavior(boolean value) {#setEnterFieldBehavior-boolean-}
```
public void setEnterFieldBehavior(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHideSelection(boolean value) {#setHideSelection-boolean-}
```
public void setHideSelection(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setListRows(int value) {#setListRows-int-}
```
public void setListRows(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setListStyle(int value) {#setListStyle-int-}
```
public void setListStyle(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setListWidth(double value) {#setListWidth-double-}
```
public void setListWidth(double value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMatchEntry(int value) {#setMatchEntry-int-}
```
public void setMatchEntry(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSelectionMargin(boolean value) {#setSelectionMargin-boolean-}
```
public void setSelectionMargin(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowColumnHeads(boolean value) {#setShowColumnHeads-boolean-}
```
public void setShowColumnHeads(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowDropButtonTypeWhen(int value) {#setShowDropButtonTypeWhen-int-}
```
public void setShowDropButtonTypeWhen(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextColumn(int value) {#setTextColumn-int-}
```
public void setTextColumn(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setValue(String value) {#setValue-java.lang.String-}
```
public void setValue(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```




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

