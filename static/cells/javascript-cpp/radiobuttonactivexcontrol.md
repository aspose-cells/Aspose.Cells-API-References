##RadioButtonActiveXControl
Represents a RadioButton ActiveX control.
## RadioButtonActiveXControl class
Represents a RadioButton ActiveX control.
```javascript
class RadioButtonActiveXControl extends ToggleButtonActiveXControl;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(ToggleButtonActiveXControl)](#constructor-togglebuttonactivexcontrol-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [groupName](#groupName--)| string | Gets and sets the group's name. |
| [alignment](#alignment--)| ControlCaptionAlignmentType | Gets and set the position of the Caption relative to the control. |
| [isWordWrapped](#isWordWrapped--)| boolean | Indicates whether the contents of the control automatically wrap at the end of a line. |
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
| [caption](#caption--)| string | Gets and set the descriptive text that appears on a control. |
| [picturePosition](#picturePosition--)| ControlPicturePositionType | Gets and set the location of the control's picture relative to its caption. |
| [specialEffect](#specialEffect--)| ControlSpecialEffectType | Gets and sets the special effect of the control. |
| [picture](#picture--)| Uint8Array | Gets and sets the data of the picture. |
| [accelerator](#accelerator--)| string | Gets and sets the accelerator key for the control. |
| [value](#value--)| CheckValueType | Indicates if the control is checked or not. |
| [isTripleState](#isTripleState--)| boolean | Indicates how the specified control will display Null values. |
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of the ActiveX control. |
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
### constructor(ToggleButtonActiveXControl) {#constructor-togglebuttonactivexcontrol-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: ToggleButtonActiveXControl);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | ToggleButtonActiveXControl | The parent object. |
### groupName {#groupName--}
Gets and sets the group's name.
```javascript
groupName : string;
```
### alignment {#alignment--}
Gets and set the position of the Caption relative to the control.
```javascript
alignment : ControlCaptionAlignmentType;
```
### isWordWrapped {#isWordWrapped--}
Indicates whether the contents of the control automatically wrap at the end of a line.
```javascript
isWordWrapped : boolean;
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
### caption {#caption--}
Gets and set the descriptive text that appears on a control.
```javascript
caption : string;
```
### picturePosition {#picturePosition--}
Gets and set the location of the control's picture relative to its caption.
```javascript
picturePosition : ControlPicturePositionType;
```
### specialEffect {#specialEffect--}
Gets and sets the special effect of the control.
```javascript
specialEffect : ControlSpecialEffectType;
```
### picture {#picture--}
Gets and sets the data of the picture.
```javascript
picture : Uint8Array;
```
### accelerator {#accelerator--}
Gets and sets the accelerator key for the control.
```javascript
accelerator : string;
```
### value {#value--}
Indicates if the control is checked or not.
```javascript
value : CheckValueType;
```
### isTripleState {#isTripleState--}
Indicates how the specified control will display Null values.
```javascript
isTripleState : boolean;
```
**Remarks**
list type="table"> <listheader> <description>Setting</description> <description>Description</description> </listheader> <item> <description>True</description> <description>The control will cycle through states for Yes, No, and Null values. The control appears dimmed (grayed) when its Value property is set to Null.</description> </item> <item> <description>False</description> <description>(Default) The control will cycle through states for Yes and No values. Null values display as if they were No values.</description> </item> </list
### getType() {#getType--}
Gets the type of the ActiveX control.
```javascript
getType() : ControlType;
```
**Returns**
[ControlType](../controltype/)
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
