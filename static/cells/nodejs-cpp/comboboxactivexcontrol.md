##ComboBoxActiveXControl
Represents a ComboBox ActiveX control.
## ComboBoxActiveXControl class
Represents a ComboBox ActiveX control.
```javascript
class ComboBoxActiveXControl extends ActiveXControl;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(ActiveXControl)](#constructor-activexcontrol-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [maxLength](#maxLength--)| number | Gets and sets the maximum number of characters |
| [listWidth](#listWidth--)| number | Gets and set the width in unit of points. |
| [boundColumn](#boundColumn--)| number | Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle). |
| [textColumn](#textColumn--)| number | Represents the column in a ComboBox or ListBox to display to the user. |
| [columnCount](#columnCount--)| number | Represents the number of columns to display in a ComboBox or ListBox. |
| [listRows](#listRows--)| number | Represents the maximum number of rows to display in the list. |
| [matchEntry](#matchEntry--)| ControlMatchEntryType | Indicates how a ListBox or ComboBox searches its list as the user types. |
| [dropButtonStyle](#dropButtonStyle--)| DropButtonStyle | Specifies the symbol displayed on the drop button |
| [showDropButtonTypeWhen](#showDropButtonTypeWhen--)| ShowDropButtonType | Specifies the symbol displayed on the drop button |
| [listStyle](#listStyle--)| ControlListStyle | Gets and sets the visual appearance. |
| [borderStyle](#borderStyle--)| ControlBorderType | Gets and set the type of border used by the control. |
| [borderOleColor](#borderOleColor--)| number | Gets and sets the ole color of the background. |
| [specialEffect](#specialEffect--)| ControlSpecialEffectType | Gets and sets the special effect of the control. |
| [isEditable](#isEditable--)| boolean | Indicates whether the user can type into the control. |
| [showColumnHeads](#showColumnHeads--)| boolean | Indicates whether column headings are displayed. |
| [isDragBehaviorEnabled](#isDragBehaviorEnabled--)| boolean | Indicates whether dragging and dropping is enabled for the control. |
| [enterFieldBehavior](#enterFieldBehavior--)| boolean | Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control. |
| [selectionMargin](#selectionMargin--)| boolean | Indicates whether the user can select a line of text by clicking in the region to the left of the text. |
| [value](#value--)| string | Gets and sets the value of the control. |
| [hideSelection](#hideSelection--)| boolean | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [columnWidths](#columnWidths--)| number | Gets and sets the width of the column. |
| [workbook](#workbook--)| Workbook | Readonly. Gets the [Workbook](../workbook/) object. |
| [mouseIcon](#mouseIcon--)| Uint8Array | Gets and sets a custom icon to display as the mouse pointer for the control. |
| [mousePointer](#mousePointer--)| ControlMousePointerType | Gets and sets the type of icon displayed as the mouse pointer for the control. |
| [linkedCell](#linkedCell--)| string | Gets and sets the linked cell. |
| [listFillRange](#listFillRange--)| string | Gets and sets the list fill range. |
| [isEnabled](#isEnabled--)| boolean | Indicates whether the control can receive the focus and respond to user-generated events. |
| [isLocked](#isLocked--)| boolean | Indicates whether data in the control is locked for editing. |
| [isTransparent](#isTransparent--)| boolean | Indicates whether the control is transparent. |
| [iMEMode](#iMEMode--)| InputMethodEditorMode | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [font](#font--)| Font | Readonly. Represents the font of the control. |
| [textAlign](#textAlign--)| TextAlignmentType | Represents how to align the text used by the control. |
## Methods
| Method | Description |
| --- | --- |
| [getMaxLength()](#getMaxLength--)| <b>@deprecated.</b> Please use the 'maxLength' property instead. Gets and sets the maximum number of characters |
| [setMaxLength(number)](#setMaxLength-number-)| <b>@deprecated.</b> Please use the 'maxLength' property instead. Gets and sets the maximum number of characters |
| [getListWidth()](#getListWidth--)| <b>@deprecated.</b> Please use the 'listWidth' property instead. Gets and set the width in unit of points. |
| [setListWidth(number)](#setListWidth-number-)| <b>@deprecated.</b> Please use the 'listWidth' property instead. Gets and set the width in unit of points. |
| [getBoundColumn()](#getBoundColumn--)| <b>@deprecated.</b> Please use the 'boundColumn' property instead. Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle). |
| [setBoundColumn(number)](#setBoundColumn-number-)| <b>@deprecated.</b> Please use the 'boundColumn' property instead. Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle). |
| [getTextColumn()](#getTextColumn--)| <b>@deprecated.</b> Please use the 'textColumn' property instead. Represents the column in a ComboBox or ListBox to display to the user. |
| [setTextColumn(number)](#setTextColumn-number-)| <b>@deprecated.</b> Please use the 'textColumn' property instead. Represents the column in a ComboBox or ListBox to display to the user. |
| [getColumnCount()](#getColumnCount--)| <b>@deprecated.</b> Please use the 'columnCount' property instead. Represents the number of columns to display in a ComboBox or ListBox. |
| [setColumnCount(number)](#setColumnCount-number-)| <b>@deprecated.</b> Please use the 'columnCount' property instead. Represents the number of columns to display in a ComboBox or ListBox. |
| [getListRows()](#getListRows--)| <b>@deprecated.</b> Please use the 'listRows' property instead. Represents the maximum number of rows to display in the list. |
| [setListRows(number)](#setListRows-number-)| <b>@deprecated.</b> Please use the 'listRows' property instead. Represents the maximum number of rows to display in the list. |
| [getMatchEntry()](#getMatchEntry--)| <b>@deprecated.</b> Please use the 'matchEntry' property instead. Indicates how a ListBox or ComboBox searches its list as the user types. |
| [setMatchEntry(ControlMatchEntryType)](#setMatchEntry-controlmatchentrytype-)| <b>@deprecated.</b> Please use the 'matchEntry' property instead. Indicates how a ListBox or ComboBox searches its list as the user types. |
| [getDropButtonStyle()](#getDropButtonStyle--)| <b>@deprecated.</b> Please use the 'dropButtonStyle' property instead. Specifies the symbol displayed on the drop button |
| [setDropButtonStyle(DropButtonStyle)](#setDropButtonStyle-dropbuttonstyle-)| <b>@deprecated.</b> Please use the 'dropButtonStyle' property instead. Specifies the symbol displayed on the drop button |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--)| <b>@deprecated.</b> Please use the 'showDropButtonTypeWhen' property instead. Specifies the symbol displayed on the drop button |
| [setShowDropButtonTypeWhen(ShowDropButtonType)](#setShowDropButtonTypeWhen-showdropbuttontype-)| <b>@deprecated.</b> Please use the 'showDropButtonTypeWhen' property instead. Specifies the symbol displayed on the drop button |
| [getListStyle()](#getListStyle--)| <b>@deprecated.</b> Please use the 'listStyle' property instead. Gets and sets the visual appearance. |
| [setListStyle(ControlListStyle)](#setListStyle-controlliststyle-)| <b>@deprecated.</b> Please use the 'listStyle' property instead. Gets and sets the visual appearance. |
| [getBorderStyle()](#getBorderStyle--)| <b>@deprecated.</b> Please use the 'borderStyle' property instead. Gets and set the type of border used by the control. |
| [setBorderStyle(ControlBorderType)](#setBorderStyle-controlbordertype-)| <b>@deprecated.</b> Please use the 'borderStyle' property instead. Gets and set the type of border used by the control. |
| [getBorderOleColor()](#getBorderOleColor--)| <b>@deprecated.</b> Please use the 'borderOleColor' property instead. Gets and sets the ole color of the background. |
| [setBorderOleColor(number)](#setBorderOleColor-number-)| <b>@deprecated.</b> Please use the 'borderOleColor' property instead. Gets and sets the ole color of the background. |
| [getSpecialEffect()](#getSpecialEffect--)| <b>@deprecated.</b> Please use the 'specialEffect' property instead. Gets and sets the special effect of the control. |
| [setSpecialEffect(ControlSpecialEffectType)](#setSpecialEffect-controlspecialeffecttype-)| <b>@deprecated.</b> Please use the 'specialEffect' property instead. Gets and sets the special effect of the control. |
| [isEditable()](#isEditable--)| <b>@deprecated.</b> Please use the 'isEditable' property instead. Indicates whether the user can type into the control. |
| [setIsEditable(boolean)](#setIsEditable-boolean-)| <b>@deprecated.</b> Please use the 'isEditable' property instead. Indicates whether the user can type into the control. |
| [getShowColumnHeads()](#getShowColumnHeads--)| <b>@deprecated.</b> Please use the 'showColumnHeads' property instead. Indicates whether column headings are displayed. |
| [setShowColumnHeads(boolean)](#setShowColumnHeads-boolean-)| <b>@deprecated.</b> Please use the 'showColumnHeads' property instead. Indicates whether column headings are displayed. |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--)| <b>@deprecated.</b> Please use the 'isDragBehaviorEnabled' property instead. Indicates whether dragging and dropping is enabled for the control. |
| [setIsDragBehaviorEnabled(boolean)](#setIsDragBehaviorEnabled-boolean-)| <b>@deprecated.</b> Please use the 'isDragBehaviorEnabled' property instead. Indicates whether dragging and dropping is enabled for the control. |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--)| <b>@deprecated.</b> Please use the 'enterFieldBehavior' property instead. Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control. |
| [setEnterFieldBehavior(boolean)](#setEnterFieldBehavior-boolean-)| <b>@deprecated.</b> Please use the 'enterFieldBehavior' property instead. Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control. |
| [getSelectionMargin()](#getSelectionMargin--)| <b>@deprecated.</b> Please use the 'selectionMargin' property instead. Indicates whether the user can select a line of text by clicking in the region to the left of the text. |
| [setSelectionMargin(boolean)](#setSelectionMargin-boolean-)| <b>@deprecated.</b> Please use the 'selectionMargin' property instead. Indicates whether the user can select a line of text by clicking in the region to the left of the text. |
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Gets and sets the value of the control. |
| [setValue(string)](#setValue-string-)| <b>@deprecated.</b> Please use the 'value' property instead. Gets and sets the value of the control. |
| [getHideSelection()](#getHideSelection--)| <b>@deprecated.</b> Please use the 'hideSelection' property instead. Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [setHideSelection(boolean)](#setHideSelection-boolean-)| <b>@deprecated.</b> Please use the 'hideSelection' property instead. Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [getColumnWidths()](#getColumnWidths--)| <b>@deprecated.</b> Please use the 'columnWidths' property instead. Gets and sets the width of the column. |
| [setColumnWidths(number)](#setColumnWidths-number-)| <b>@deprecated.</b> Please use the 'columnWidths' property instead. Gets and sets the width of the column. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getWorkbook()](#getWorkbook--)| <b>@deprecated.</b> Please use the 'workbook' property instead. Gets the [Workbook](../workbook/) object. |
| [getMouseIcon()](#getMouseIcon--)| <b>@deprecated.</b> Please use the 'mouseIcon' property instead. Gets and sets a custom icon to display as the mouse pointer for the control. |
| [setMouseIcon(Uint8Array)](#setMouseIcon-uint8array-)| <b>@deprecated.</b> Please use the 'mouseIcon' property instead. Gets and sets a custom icon to display as the mouse pointer for the control. |
| [getMousePointer()](#getMousePointer--)| <b>@deprecated.</b> Please use the 'mousePointer' property instead. Gets and sets the type of icon displayed as the mouse pointer for the control. |
| [setMousePointer(ControlMousePointerType)](#setMousePointer-controlmousepointertype-)| <b>@deprecated.</b> Please use the 'mousePointer' property instead. Gets and sets the type of icon displayed as the mouse pointer for the control. |
| [getLinkedCell()](#getLinkedCell--)| <b>@deprecated.</b> Please use the 'linkedCell' property instead. Gets and sets the linked cell. |
| [setLinkedCell(string)](#setLinkedCell-string-)| <b>@deprecated.</b> Please use the 'linkedCell' property instead. Gets and sets the linked cell. |
| [getListFillRange()](#getListFillRange--)| <b>@deprecated.</b> Please use the 'listFillRange' property instead. Gets and sets the list fill range. |
| [setListFillRange(string)](#setListFillRange-string-)| <b>@deprecated.</b> Please use the 'listFillRange' property instead. Gets and sets the list fill range. |
| [isEnabled()](#isEnabled--)| <b>@deprecated.</b> Please use the 'isEnabled' property instead. Indicates whether the control can receive the focus and respond to user-generated events. |
| [setIsEnabled(boolean)](#setIsEnabled-boolean-)| <b>@deprecated.</b> Please use the 'isEnabled' property instead. Indicates whether the control can receive the focus and respond to user-generated events. |
| [isLocked()](#isLocked--)| <b>@deprecated.</b> Please use the 'isLocked' property instead. Indicates whether data in the control is locked for editing. |
| [setIsLocked(boolean)](#setIsLocked-boolean-)| <b>@deprecated.</b> Please use the 'isLocked' property instead. Indicates whether data in the control is locked for editing. |
| [isTransparent()](#isTransparent--)| <b>@deprecated.</b> Please use the 'isTransparent' property instead. Indicates whether the control is transparent. |
| [setIsTransparent(boolean)](#setIsTransparent-boolean-)| <b>@deprecated.</b> Please use the 'isTransparent' property instead. Indicates whether the control is transparent. |
| [getIMEMode()](#getIMEMode--)| <b>@deprecated.</b> Please use the 'iMEMode' property instead. Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [setIMEMode(InputMethodEditorMode)](#setIMEMode-inputmethodeditormode-)| <b>@deprecated.</b> Please use the 'iMEMode' property instead. Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [getFont()](#getFont--)| <b>@deprecated.</b> Please use the 'font' property instead. Represents the font of the control. |
| [getTextAlign()](#getTextAlign--)| <b>@deprecated.</b> Please use the 'textAlign' property instead. Represents how to align the text used by the control. |
| [setTextAlign(TextAlignmentType)](#setTextAlign-textalignmenttype-)| <b>@deprecated.</b> Please use the 'textAlign' property instead. Represents how to align the text used by the control. |
| [getType()](#getType--)| Gets the type of the ActiveX control. |
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
| [getData()](#getData--)| Gets and sets the binary data of the control. |
### constructor(ActiveXControl) {#constructor-activexcontrol-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: ActiveXControl);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | ActiveXControl | The parent object. |
### maxLength {#maxLength--}
Gets and sets the maximum number of characters
```javascript
maxLength : number;
```
### listWidth {#listWidth--}
Gets and set the width in unit of points.
```javascript
listWidth : number;
```
### boundColumn {#boundColumn--}
Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle).
```javascript
boundColumn : number;
```
### textColumn {#textColumn--}
Represents the column in a ComboBox or ListBox to display to the user.
```javascript
textColumn : number;
```
### columnCount {#columnCount--}
Represents the number of columns to display in a ComboBox or ListBox.
```javascript
columnCount : number;
```
### listRows {#listRows--}
Represents the maximum number of rows to display in the list.
```javascript
listRows : number;
```
### matchEntry {#matchEntry--}
Indicates how a ListBox or ComboBox searches its list as the user types.
```javascript
matchEntry : ControlMatchEntryType;
```
### dropButtonStyle {#dropButtonStyle--}
Specifies the symbol displayed on the drop button
```javascript
dropButtonStyle : DropButtonStyle;
```
### showDropButtonTypeWhen {#showDropButtonTypeWhen--}
Specifies the symbol displayed on the drop button
```javascript
showDropButtonTypeWhen : ShowDropButtonType;
```
### listStyle {#listStyle--}
Gets and sets the visual appearance.
```javascript
listStyle : ControlListStyle;
```
### borderStyle {#borderStyle--}
Gets and set the type of border used by the control.
```javascript
borderStyle : ControlBorderType;
```
### borderOleColor {#borderOleColor--}
Gets and sets the ole color of the background.
```javascript
borderOleColor : number;
```
### specialEffect {#specialEffect--}
Gets and sets the special effect of the control.
```javascript
specialEffect : ControlSpecialEffectType;
```
### isEditable {#isEditable--}
Indicates whether the user can type into the control.
```javascript
isEditable : boolean;
```
### showColumnHeads {#showColumnHeads--}
Indicates whether column headings are displayed.
```javascript
showColumnHeads : boolean;
```
### isDragBehaviorEnabled {#isDragBehaviorEnabled--}
Indicates whether dragging and dropping is enabled for the control.
```javascript
isDragBehaviorEnabled : boolean;
```
### enterFieldBehavior {#enterFieldBehavior--}
Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control.
```javascript
enterFieldBehavior : boolean;
```
### selectionMargin {#selectionMargin--}
Indicates whether the user can select a line of text by clicking in the region to the left of the text.
```javascript
selectionMargin : boolean;
```
### value {#value--}
Gets and sets the value of the control.
```javascript
value : string;
```
### hideSelection {#hideSelection--}
Indicates whether selected text in the control appears highlighted when the control does not have focus.
```javascript
hideSelection : boolean;
```
### columnWidths {#columnWidths--}
Gets and sets the width of the column.
```javascript
columnWidths : number;
```
### workbook {#workbook--}
Readonly. Gets the [Workbook](../workbook/) object.
```javascript
workbook : Workbook;
```
### mouseIcon {#mouseIcon--}
Gets and sets a custom icon to display as the mouse pointer for the control.
```javascript
mouseIcon : Uint8Array;
```
### mousePointer {#mousePointer--}
Gets and sets the type of icon displayed as the mouse pointer for the control.
```javascript
mousePointer : ControlMousePointerType;
```
### linkedCell {#linkedCell--}
Gets and sets the linked cell.
```javascript
linkedCell : string;
```
### listFillRange {#listFillRange--}
Gets and sets the list fill range.
```javascript
listFillRange : string;
```
### isEnabled {#isEnabled--}
Indicates whether the control can receive the focus and respond to user-generated events.
```javascript
isEnabled : boolean;
```
### isLocked {#isLocked--}
Indicates whether data in the control is locked for editing.
```javascript
isLocked : boolean;
```
### isTransparent {#isTransparent--}
Indicates whether the control is transparent.
```javascript
isTransparent : boolean;
```
### iMEMode {#iMEMode--}
Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus.
```javascript
iMEMode : InputMethodEditorMode;
```
### font {#font--}
Readonly. Represents the font of the control.
```javascript
font : Font;
```
### textAlign {#textAlign--}
Represents how to align the text used by the control.
```javascript
textAlign : TextAlignmentType;
```
### getMaxLength() {#getMaxLength--}
```javascript
getMaxLength() : number;
```
### setMaxLength(number) {#setMaxLength-number-}
```javascript
setMaxLength(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getListWidth() {#getListWidth--}
```javascript
getListWidth() : number;
```
### setListWidth(number) {#setListWidth-number-}
```javascript
setListWidth(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getBoundColumn() {#getBoundColumn--}
```javascript
getBoundColumn() : number;
```
### setBoundColumn(number) {#setBoundColumn-number-}
```javascript
setBoundColumn(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getTextColumn() {#getTextColumn--}
```javascript
getTextColumn() : number;
```
### setTextColumn(number) {#setTextColumn-number-}
```javascript
setTextColumn(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getColumnCount() {#getColumnCount--}
```javascript
getColumnCount() : number;
```
### setColumnCount(number) {#setColumnCount-number-}
```javascript
setColumnCount(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getListRows() {#getListRows--}
```javascript
getListRows() : number;
```
### setListRows(number) {#setListRows-number-}
```javascript
setListRows(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getMatchEntry() {#getMatchEntry--}
```javascript
getMatchEntry() : ControlMatchEntryType;
```
**Returns**
[ControlMatchEntryType](../controlmatchentrytype/)
### setMatchEntry(ControlMatchEntryType) {#setMatchEntry-controlmatchentrytype-}
```javascript
setMatchEntry(value: ControlMatchEntryType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ControlMatchEntryType](../controlmatchentrytype/) | The value to set. |
### getDropButtonStyle() {#getDropButtonStyle--}
```javascript
getDropButtonStyle() : DropButtonStyle;
```
**Returns**
[DropButtonStyle](../dropbuttonstyle/)
### setDropButtonStyle(DropButtonStyle) {#setDropButtonStyle-dropbuttonstyle-}
```javascript
setDropButtonStyle(value: DropButtonStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DropButtonStyle](../dropbuttonstyle/) | The value to set. |
### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}
```javascript
getShowDropButtonTypeWhen() : ShowDropButtonType;
```
**Returns**
[ShowDropButtonType](../showdropbuttontype/)
### setShowDropButtonTypeWhen(ShowDropButtonType) {#setShowDropButtonTypeWhen-showdropbuttontype-}
```javascript
setShowDropButtonTypeWhen(value: ShowDropButtonType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ShowDropButtonType](../showdropbuttontype/) | The value to set. |
### getListStyle() {#getListStyle--}
```javascript
getListStyle() : ControlListStyle;
```
**Returns**
[ControlListStyle](../controlliststyle/)
### setListStyle(ControlListStyle) {#setListStyle-controlliststyle-}
```javascript
setListStyle(value: ControlListStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ControlListStyle](../controlliststyle/) | The value to set. |
### getBorderStyle() {#getBorderStyle--}
```javascript
getBorderStyle() : ControlBorderType;
```
**Returns**
[ControlBorderType](../controlbordertype/)
### setBorderStyle(ControlBorderType) {#setBorderStyle-controlbordertype-}
```javascript
setBorderStyle(value: ControlBorderType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ControlBorderType](../controlbordertype/) | The value to set. |
### getBorderOleColor() {#getBorderOleColor--}
```javascript
getBorderOleColor() : number;
```
### setBorderOleColor(number) {#setBorderOleColor-number-}
```javascript
setBorderOleColor(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getSpecialEffect() {#getSpecialEffect--}
```javascript
getSpecialEffect() : ControlSpecialEffectType;
```
**Returns**
[ControlSpecialEffectType](../controlspecialeffecttype/)
### setSpecialEffect(ControlSpecialEffectType) {#setSpecialEffect-controlspecialeffecttype-}
```javascript
setSpecialEffect(value: ControlSpecialEffectType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ControlSpecialEffectType](../controlspecialeffecttype/) | The value to set. |
### isEditable() {#isEditable--}
```javascript
isEditable() : boolean;
```
### setIsEditable(boolean) {#setIsEditable-boolean-}
```javascript
setIsEditable(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowColumnHeads() {#getShowColumnHeads--}
```javascript
getShowColumnHeads() : boolean;
```
### setShowColumnHeads(boolean) {#setShowColumnHeads-boolean-}
```javascript
setShowColumnHeads(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isDragBehaviorEnabled() {#isDragBehaviorEnabled--}
```javascript
isDragBehaviorEnabled() : boolean;
```
### setIsDragBehaviorEnabled(boolean) {#setIsDragBehaviorEnabled-boolean-}
```javascript
setIsDragBehaviorEnabled(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getEnterFieldBehavior() {#getEnterFieldBehavior--}
```javascript
getEnterFieldBehavior() : boolean;
```
### setEnterFieldBehavior(boolean) {#setEnterFieldBehavior-boolean-}
```javascript
setEnterFieldBehavior(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getSelectionMargin() {#getSelectionMargin--}
```javascript
getSelectionMargin() : boolean;
```
### setSelectionMargin(boolean) {#setSelectionMargin-boolean-}
```javascript
setSelectionMargin(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getValue() {#getValue--}
```javascript
getValue() : string;
```
### setValue(string) {#setValue-string-}
```javascript
setValue(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getHideSelection() {#getHideSelection--}
```javascript
getHideSelection() : boolean;
```
### setHideSelection(boolean) {#setHideSelection-boolean-}
```javascript
setHideSelection(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getColumnWidths() {#getColumnWidths--}
```javascript
getColumnWidths() : number;
```
### setColumnWidths(number) {#setColumnWidths-number-}
```javascript
setColumnWidths(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getWorkbook() {#getWorkbook--}
```javascript
getWorkbook() : Workbook;
```
**Returns**
[Workbook](../workbook/)
### getMouseIcon() {#getMouseIcon--}
```javascript
getMouseIcon() : Uint8Array;
```
### setMouseIcon(Uint8Array) {#setMouseIcon-uint8array-}
```javascript
setMouseIcon(value: Uint8Array) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |
### getMousePointer() {#getMousePointer--}
```javascript
getMousePointer() : ControlMousePointerType;
```
**Returns**
[ControlMousePointerType](../controlmousepointertype/)
### setMousePointer(ControlMousePointerType) {#setMousePointer-controlmousepointertype-}
```javascript
setMousePointer(value: ControlMousePointerType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ControlMousePointerType](../controlmousepointertype/) | The value to set. |
### getLinkedCell() {#getLinkedCell--}
```javascript
getLinkedCell() : string;
```
### setLinkedCell(string) {#setLinkedCell-string-}
```javascript
setLinkedCell(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getListFillRange() {#getListFillRange--}
```javascript
getListFillRange() : string;
```
### setListFillRange(string) {#setListFillRange-string-}
```javascript
setListFillRange(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isEnabled() {#isEnabled--}
```javascript
isEnabled() : boolean;
```
### setIsEnabled(boolean) {#setIsEnabled-boolean-}
```javascript
setIsEnabled(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isLocked() {#isLocked--}
```javascript
isLocked() : boolean;
```
### setIsLocked(boolean) {#setIsLocked-boolean-}
```javascript
setIsLocked(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isTransparent() {#isTransparent--}
```javascript
isTransparent() : boolean;
```
### setIsTransparent(boolean) {#setIsTransparent-boolean-}
```javascript
setIsTransparent(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getIMEMode() {#getIMEMode--}
```javascript
getIMEMode() : InputMethodEditorMode;
```
**Returns**
[InputMethodEditorMode](../inputmethodeditormode/)
### setIMEMode(InputMethodEditorMode) {#setIMEMode-inputmethodeditormode-}
```javascript
setIMEMode(value: InputMethodEditorMode) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [InputMethodEditorMode](../inputmethodeditormode/) | The value to set. |
### getFont() {#getFont--}
```javascript
getFont() : Font;
```
**Returns**
[Font](../font/)
### getTextAlign() {#getTextAlign--}
```javascript
getTextAlign() : TextAlignmentType;
```
**Returns**
[TextAlignmentType](../textalignmenttype/)
### setTextAlign(TextAlignmentType) {#setTextAlign-textalignmenttype-}
```javascript
setTextAlign(value: TextAlignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |
### getType() {#getType--}
Gets the type of the ActiveX control.
```javascript
getType() : ControlType;
```
**Returns**
[ControlType](../controltype/)
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
### getData() {#getData--}
Gets and sets the binary data of the control.
```javascript
getData() : Uint8Array;
```
