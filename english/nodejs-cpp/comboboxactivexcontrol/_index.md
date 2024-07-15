---
title: ComboBoxActiveXControl
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a ComboBox ActiveX control.
type: docs
url: /nodejs-cpp/comboboxactivexcontrol/
---

## ComboBoxActiveXControl class

Represents a ComboBox ActiveX control.

```javascript
class ComboBoxActiveXControl extends ActiveXControl;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(ActiveXControl)](#constructor-activexcontrol-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of the ActiveX control. |
| [getMaxLength()](#getMaxLength--)| Gets and sets the maximum number of characters |
| [setMaxLength(number)](#setMaxLength-number-)| Gets and sets the maximum number of characters |
| [getListWidth()](#getListWidth--)| Gets and set the width in unit of points. |
| [setListWidth(number)](#setListWidth-number-)| Gets and set the width in unit of points. |
| [getBoundColumn()](#getBoundColumn--)| Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle). |
| [setBoundColumn(number)](#setBoundColumn-number-)| Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle). |
| [getTextColumn()](#getTextColumn--)| Represents the column in a ComboBox or ListBox to display to the user. |
| [setTextColumn(number)](#setTextColumn-number-)| Represents the column in a ComboBox or ListBox to display to the user. |
| [getColumnCount()](#getColumnCount--)| Represents the number of columns to display in a ComboBox or ListBox. |
| [setColumnCount(number)](#setColumnCount-number-)| Represents the number of columns to display in a ComboBox or ListBox. |
| [getListRows()](#getListRows--)| Represents the maximum number of rows to display in the list. |
| [setListRows(number)](#setListRows-number-)| Represents the maximum number of rows to display in the list. |
| [getMatchEntry()](#getMatchEntry--)| Indicates how a ListBox or ComboBox searches its list as the user types. |
| [setMatchEntry(ControlMatchEntryType)](#setMatchEntry-controlmatchentrytype-)| Indicates how a ListBox or ComboBox searches its list as the user types. |
| [getDropButtonStyle()](#getDropButtonStyle--)| Specifies the symbol displayed on the drop button |
| [setDropButtonStyle(DropButtonStyle)](#setDropButtonStyle-dropbuttonstyle-)| Specifies the symbol displayed on the drop button |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--)| Specifies the symbol displayed on the drop button |
| [setShowDropButtonTypeWhen(ShowDropButtonType)](#setShowDropButtonTypeWhen-showdropbuttontype-)| Specifies the symbol displayed on the drop button |
| [getListStyle()](#getListStyle--)| Gets and sets the visual appearance. |
| [setListStyle(ControlListStyle)](#setListStyle-controlliststyle-)| Gets and sets the visual appearance. |
| [getBorderStyle()](#getBorderStyle--)| Gets and set the type of border used by the control. |
| [setBorderStyle(ControlBorderType)](#setBorderStyle-controlbordertype-)| Gets and set the type of border used by the control. |
| [getBorderOleColor()](#getBorderOleColor--)| Gets and sets the ole color of the background. |
| [setBorderOleColor(number)](#setBorderOleColor-number-)| Gets and sets the ole color of the background. |
| [getSpecialEffect()](#getSpecialEffect--)| Gets and sets the special effect of the control. |
| [setSpecialEffect(ControlSpecialEffectType)](#setSpecialEffect-controlspecialeffecttype-)| Gets and sets the special effect of the control. |
| [isEditable()](#isEditable--)| Indicates whether the user can type into the control. |
| [setIsEditable(boolean)](#setIsEditable-boolean-)| Indicates whether the user can type into the control. |
| [getShowColumnHeads()](#getShowColumnHeads--)| Indicates whether column headings are displayed. |
| [setShowColumnHeads(boolean)](#setShowColumnHeads-boolean-)| Indicates whether column headings are displayed. |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--)| Indicates whether dragging and dropping is enabled for the control. |
| [setIsDragBehaviorEnabled(boolean)](#setIsDragBehaviorEnabled-boolean-)| Indicates whether dragging and dropping is enabled for the control. |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--)| Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control. |
| [setEnterFieldBehavior(boolean)](#setEnterFieldBehavior-boolean-)| Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control. |
| [getSelectionMargin()](#getSelectionMargin--)| Indicates whether the user can select a line of text by clicking in the region to the left of the text. |
| [setSelectionMargin(boolean)](#setSelectionMargin-boolean-)| Indicates whether the user can select a line of text by clicking in the region to the left of the text. |
| [getValue()](#getValue--)| Gets and sets the value of the control. |
| [setValue(string)](#setValue-string-)| Gets and sets the value of the control. |
| [getHideSelection()](#getHideSelection--)| Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [setHideSelection(boolean)](#setHideSelection-boolean-)| Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [getColumnWidths()](#getColumnWidths--)| Gets and sets the width of the column. |
| [setColumnWidths(number)](#setColumnWidths-number-)| Gets and sets the width of the column. |
| [getWorkbook()](#getWorkbook--)| Gets the [Workbook](../workbook/) object. |
| [getMouseIcon()](#getMouseIcon--)| Gets and sets a custom icon to display as the mouse pointer for the control. |
| [setMouseIcon(number[])](#setMouseIcon-numberarray-)| Gets and sets a custom icon to display as the mouse pointer for the control. |
| [getMousePointer()](#getMousePointer--)| Gets and sets the type of icon displayed as the mouse pointer for the control. |
| [setMousePointer(ControlMousePointerType)](#setMousePointer-controlmousepointertype-)| Gets and sets the type of icon displayed as the mouse pointer for the control. |
| [getLinkedCell()](#getLinkedCell--)| Gets and sets the linked cell. |
| [setLinkedCell(string)](#setLinkedCell-string-)| Gets and sets the linked cell. |
| [getListFillRange()](#getListFillRange--)| Gets and sets the list fill range. |
| [setListFillRange(string)](#setListFillRange-string-)| Gets and sets the list fill range. |
| [isEnabled()](#isEnabled--)| Indicates whether the control can receive the focus and respond to user-generated events. |
| [setIsEnabled(boolean)](#setIsEnabled-boolean-)| Indicates whether the control can receive the focus and respond to user-generated events. |
| [isLocked()](#isLocked--)| Indicates whether data in the control is locked for editing. |
| [setIsLocked(boolean)](#setIsLocked-boolean-)| Indicates whether data in the control is locked for editing. |
| [isTransparent()](#isTransparent--)| Indicates whether the control is transparent. |
| [setIsTransparent(boolean)](#setIsTransparent-boolean-)| Indicates whether the control is transparent. |
| [getIMEMode()](#getIMEMode--)| Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [setIMEMode(InputMethodEditorMode)](#setIMEMode-inputmethodeditormode-)| Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [getFont()](#getFont--)| Represents the font of the control. |
| [getTextAlign()](#getTextAlign--)| Represents how to align the text used by the control. |
| [setTextAlign(TextAlignmentType)](#setTextAlign-textalignmenttype-)| Represents how to align the text used by the control. |
| [getData()](#getData--)| Gets and sets the binary data of the control. |
| [isAutoWordSelected()](#isAutoWordSelected--)| Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false specifies that the basic unit is a whole word. |
| [setIsAutoWordSelected(boolean)](#setIsAutoWordSelected-boolean-)| Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false specifies that the basic unit is a whole word. |
| [getWidth()](#getWidth--)| Gets and sets the width of the control in unit of points. |
| [setWidth(number)](#setWidth-number-)| Gets and sets the width of the control in unit of points. |
| [getHeight()](#getHeight--)| Gets and sets the height of the control in unit of points. |
| [setHeight(number)](#setHeight-number-)| Gets and sets the height of the control in unit of points. |
| [getForeOleColor()](#getForeOleColor--)| Gets and sets the ole color of the foreground. |
| [setForeOleColor(number)](#setForeOleColor-number-)| Gets and sets the ole color of the foreground. |
| [getBackOleColor()](#getBackOleColor--)| Gets and sets the ole color of the background. |
| [setBackOleColor(number)](#setBackOleColor-number-)| Gets and sets the ole color of the background. |
| [isVisible()](#isVisible--)| Indicates whether this control is visible. |
| [setIsVisible(boolean)](#setIsVisible-boolean-)| Indicates whether this control is visible. |
| [getShadow()](#getShadow--)| Indicates whether to show a shadow. |
| [setShadow(boolean)](#setShadow-boolean-)| Indicates whether to show a shadow. |
| [isAutoSize()](#isAutoSize--)| Indicates whether the control will automatically resize to display its entire contents. |
| [setIsAutoSize(boolean)](#setIsAutoSize-boolean-)| Indicates whether the control will automatically resize to display its entire contents. |


### constructor(ActiveXControl) {#constructor-activexcontrol-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: ActiveXControl);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | ActiveXControl | The parent object. |

### getType() {#getType--}

Gets the type of the ActiveX control.

```javascript
getType() : ControlType;
```


**Returns**

[ControlType](../controltype/)

### getMaxLength() {#getMaxLength--}

Gets and sets the maximum number of characters

```javascript
getMaxLength() : number;
```


### setMaxLength(number) {#setMaxLength-number-}

Gets and sets the maximum number of characters

```javascript
setMaxLength(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getListWidth() {#getListWidth--}

Gets and set the width in unit of points.

```javascript
getListWidth() : number;
```


### setListWidth(number) {#setListWidth-number-}

Gets and set the width in unit of points.

```javascript
setListWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getBoundColumn() {#getBoundColumn--}

Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle).

```javascript
getBoundColumn() : number;
```


### setBoundColumn(number) {#setBoundColumn-number-}

Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle).

```javascript
setBoundColumn(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTextColumn() {#getTextColumn--}

Represents the column in a ComboBox or ListBox to display to the user.

```javascript
getTextColumn() : number;
```


### setTextColumn(number) {#setTextColumn-number-}

Represents the column in a ComboBox or ListBox to display to the user.

```javascript
setTextColumn(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getColumnCount() {#getColumnCount--}

Represents the number of columns to display in a ComboBox or ListBox.

```javascript
getColumnCount() : number;
```


### setColumnCount(number) {#setColumnCount-number-}

Represents the number of columns to display in a ComboBox or ListBox.

```javascript
setColumnCount(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getListRows() {#getListRows--}

Represents the maximum number of rows to display in the list.

```javascript
getListRows() : number;
```


### setListRows(number) {#setListRows-number-}

Represents the maximum number of rows to display in the list.

```javascript
setListRows(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getMatchEntry() {#getMatchEntry--}

Indicates how a ListBox or ComboBox searches its list as the user types.

```javascript
getMatchEntry() : ControlMatchEntryType;
```


**Returns**

[ControlMatchEntryType](../controlmatchentrytype/)

### setMatchEntry(ControlMatchEntryType) {#setMatchEntry-controlmatchentrytype-}

Indicates how a ListBox or ComboBox searches its list as the user types.

```javascript
setMatchEntry(value: ControlMatchEntryType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ControlMatchEntryType](../controlmatchentrytype/) | The value to set. |

### getDropButtonStyle() {#getDropButtonStyle--}

Specifies the symbol displayed on the drop button

```javascript
getDropButtonStyle() : DropButtonStyle;
```


**Returns**

[DropButtonStyle](../dropbuttonstyle/)

### setDropButtonStyle(DropButtonStyle) {#setDropButtonStyle-dropbuttonstyle-}

Specifies the symbol displayed on the drop button

```javascript
setDropButtonStyle(value: DropButtonStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DropButtonStyle](../dropbuttonstyle/) | The value to set. |

### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}

Specifies the symbol displayed on the drop button

```javascript
getShowDropButtonTypeWhen() : ShowDropButtonType;
```


**Returns**

[ShowDropButtonType](../showdropbuttontype/)

### setShowDropButtonTypeWhen(ShowDropButtonType) {#setShowDropButtonTypeWhen-showdropbuttontype-}

Specifies the symbol displayed on the drop button

```javascript
setShowDropButtonTypeWhen(value: ShowDropButtonType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ShowDropButtonType](../showdropbuttontype/) | The value to set. |

### getListStyle() {#getListStyle--}

Gets and sets the visual appearance.

```javascript
getListStyle() : ControlListStyle;
```


**Returns**

[ControlListStyle](../controlliststyle/)

### setListStyle(ControlListStyle) {#setListStyle-controlliststyle-}

Gets and sets the visual appearance.

```javascript
setListStyle(value: ControlListStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ControlListStyle](../controlliststyle/) | The value to set. |

### getBorderStyle() {#getBorderStyle--}

Gets and set the type of border used by the control.

```javascript
getBorderStyle() : ControlBorderType;
```


**Returns**

[ControlBorderType](../controlbordertype/)

### setBorderStyle(ControlBorderType) {#setBorderStyle-controlbordertype-}

Gets and set the type of border used by the control.

```javascript
setBorderStyle(value: ControlBorderType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ControlBorderType](../controlbordertype/) | The value to set. |

### getBorderOleColor() {#getBorderOleColor--}

Gets and sets the ole color of the background.

```javascript
getBorderOleColor() : number;
```


### setBorderOleColor(number) {#setBorderOleColor-number-}

Gets and sets the ole color of the background.

```javascript
setBorderOleColor(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getSpecialEffect() {#getSpecialEffect--}

Gets and sets the special effect of the control.

```javascript
getSpecialEffect() : ControlSpecialEffectType;
```


**Returns**

[ControlSpecialEffectType](../controlspecialeffecttype/)

### setSpecialEffect(ControlSpecialEffectType) {#setSpecialEffect-controlspecialeffecttype-}

Gets and sets the special effect of the control.

```javascript
setSpecialEffect(value: ControlSpecialEffectType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ControlSpecialEffectType](../controlspecialeffecttype/) | The value to set. |

### isEditable() {#isEditable--}

Indicates whether the user can type into the control.

```javascript
isEditable() : boolean;
```


### setIsEditable(boolean) {#setIsEditable-boolean-}

Indicates whether the user can type into the control.

```javascript
setIsEditable(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowColumnHeads() {#getShowColumnHeads--}

Indicates whether column headings are displayed.

```javascript
getShowColumnHeads() : boolean;
```


### setShowColumnHeads(boolean) {#setShowColumnHeads-boolean-}

Indicates whether column headings are displayed.

```javascript
setShowColumnHeads(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isDragBehaviorEnabled() {#isDragBehaviorEnabled--}

Indicates whether dragging and dropping is enabled for the control.

```javascript
isDragBehaviorEnabled() : boolean;
```


### setIsDragBehaviorEnabled(boolean) {#setIsDragBehaviorEnabled-boolean-}

Indicates whether dragging and dropping is enabled for the control.

```javascript
setIsDragBehaviorEnabled(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEnterFieldBehavior() {#getEnterFieldBehavior--}

Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control.

```javascript
getEnterFieldBehavior() : boolean;
```


### setEnterFieldBehavior(boolean) {#setEnterFieldBehavior-boolean-}

Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control.

```javascript
setEnterFieldBehavior(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSelectionMargin() {#getSelectionMargin--}

Indicates whether the user can select a line of text by clicking in the region to the left of the text.

```javascript
getSelectionMargin() : boolean;
```


### setSelectionMargin(boolean) {#setSelectionMargin-boolean-}

Indicates whether the user can select a line of text by clicking in the region to the left of the text.

```javascript
setSelectionMargin(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getValue() {#getValue--}

Gets and sets the value of the control.

```javascript
getValue() : string;
```


### setValue(string) {#setValue-string-}

Gets and sets the value of the control.

```javascript
setValue(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getHideSelection() {#getHideSelection--}

Indicates whether selected text in the control appears highlighted when the control does not have focus.

```javascript
getHideSelection() : boolean;
```


### setHideSelection(boolean) {#setHideSelection-boolean-}

Indicates whether selected text in the control appears highlighted when the control does not have focus.

```javascript
setHideSelection(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getColumnWidths() {#getColumnWidths--}

Gets and sets the width of the column.

```javascript
getColumnWidths() : number;
```


### setColumnWidths(number) {#setColumnWidths-number-}

Gets and sets the width of the column.

```javascript
setColumnWidths(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWorkbook() {#getWorkbook--}

Gets the [Workbook](../workbook/) object.

```javascript
getWorkbook() : Workbook;
```


**Returns**

[Workbook](../workbook/)

### getMouseIcon() {#getMouseIcon--}

Gets and sets a custom icon to display as the mouse pointer for the control.

```javascript
getMouseIcon() : number[];
```


**Returns**

number[]

### setMouseIcon(number[]) {#setMouseIcon-numberarray-}

Gets and sets a custom icon to display as the mouse pointer for the control.

```javascript
setMouseIcon(value: number[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### getMousePointer() {#getMousePointer--}

Gets and sets the type of icon displayed as the mouse pointer for the control.

```javascript
getMousePointer() : ControlMousePointerType;
```


**Returns**

[ControlMousePointerType](../controlmousepointertype/)

### setMousePointer(ControlMousePointerType) {#setMousePointer-controlmousepointertype-}

Gets and sets the type of icon displayed as the mouse pointer for the control.

```javascript
setMousePointer(value: ControlMousePointerType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ControlMousePointerType](../controlmousepointertype/) | The value to set. |

### getLinkedCell() {#getLinkedCell--}

Gets and sets the linked cell.

```javascript
getLinkedCell() : string;
```


### setLinkedCell(string) {#setLinkedCell-string-}

Gets and sets the linked cell.

```javascript
setLinkedCell(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getListFillRange() {#getListFillRange--}

Gets and sets the list fill range.

```javascript
getListFillRange() : string;
```


### setListFillRange(string) {#setListFillRange-string-}

Gets and sets the list fill range.

```javascript
setListFillRange(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isEnabled() {#isEnabled--}

Indicates whether the control can receive the focus and respond to user-generated events.

```javascript
isEnabled() : boolean;
```


### setIsEnabled(boolean) {#setIsEnabled-boolean-}

Indicates whether the control can receive the focus and respond to user-generated events.

```javascript
setIsEnabled(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isLocked() {#isLocked--}

Indicates whether data in the control is locked for editing.

```javascript
isLocked() : boolean;
```


### setIsLocked(boolean) {#setIsLocked-boolean-}

Indicates whether data in the control is locked for editing.

```javascript
setIsLocked(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isTransparent() {#isTransparent--}

Indicates whether the control is transparent.

```javascript
isTransparent() : boolean;
```


### setIsTransparent(boolean) {#setIsTransparent-boolean-}

Indicates whether the control is transparent.

```javascript
setIsTransparent(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getIMEMode() {#getIMEMode--}

Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus.

```javascript
getIMEMode() : InputMethodEditorMode;
```


**Returns**

[InputMethodEditorMode](../inputmethodeditormode/)

### setIMEMode(InputMethodEditorMode) {#setIMEMode-inputmethodeditormode-}

Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus.

```javascript
setIMEMode(value: InputMethodEditorMode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [InputMethodEditorMode](../inputmethodeditormode/) | The value to set. |

### getFont() {#getFont--}

Represents the font of the control.

```javascript
getFont() : Font;
```


**Returns**

[Font](../font/)

### getTextAlign() {#getTextAlign--}

Represents how to align the text used by the control.

```javascript
getTextAlign() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](../textalignmenttype/)

### setTextAlign(TextAlignmentType) {#setTextAlign-textalignmenttype-}

Represents how to align the text used by the control.

```javascript
setTextAlign(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |

### getData() {#getData--}

Gets and sets the binary data of the control.

```javascript
getData() : number[];
```


**Returns**

number[]

### isAutoWordSelected() {#isAutoWordSelected--}

Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false specifies that the basic unit is a whole word.

```javascript
isAutoWordSelected() : boolean;
```


### setIsAutoWordSelected(boolean) {#setIsAutoWordSelected-boolean-}

Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false specifies that the basic unit is a whole word.

```javascript
setIsAutoWordSelected(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getWidth() {#getWidth--}

Gets and sets the width of the control in unit of points.

```javascript
getWidth() : number;
```


### setWidth(number) {#setWidth-number-}

Gets and sets the width of the control in unit of points.

```javascript
setWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeight() {#getHeight--}

Gets and sets the height of the control in unit of points.

```javascript
getHeight() : number;
```


### setHeight(number) {#setHeight-number-}

Gets and sets the height of the control in unit of points.

```javascript
setHeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getForeOleColor() {#getForeOleColor--}

Gets and sets the ole color of the foreground.

```javascript
getForeOleColor() : number;
```


**Remarks**

Not applies to Image control.

### setForeOleColor(number) {#setForeOleColor-number-}

Gets and sets the ole color of the foreground.

```javascript
setForeOleColor(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Not applies to Image control.

### getBackOleColor() {#getBackOleColor--}

Gets and sets the ole color of the background.

```javascript
getBackOleColor() : number;
```


### setBackOleColor(number) {#setBackOleColor-number-}

Gets and sets the ole color of the background.

```javascript
setBackOleColor(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isVisible() {#isVisible--}

Indicates whether this control is visible.

```javascript
isVisible() : boolean;
```


### setIsVisible(boolean) {#setIsVisible-boolean-}

Indicates whether this control is visible.

```javascript
setIsVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShadow() {#getShadow--}

Indicates whether to show a shadow.

```javascript
getShadow() : boolean;
```


### setShadow(boolean) {#setShadow-boolean-}

Indicates whether to show a shadow.

```javascript
setShadow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isAutoSize() {#isAutoSize--}

Indicates whether the control will automatically resize to display its entire contents.

```javascript
isAutoSize() : boolean;
```


### setIsAutoSize(boolean) {#setIsAutoSize-boolean-}

Indicates whether the control will automatically resize to display its entire contents.

```javascript
setIsAutoSize(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |


