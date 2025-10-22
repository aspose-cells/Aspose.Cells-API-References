##ComboBoxActiveXControl
Represents a ComboBox ActiveX control.
## ComboBoxActiveXControl class
Represents a ComboBox ActiveX control.
```javascript
class ComboBoxActiveXControl extends ActiveXControl;
```
## Constructors
| Name | Description |
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
