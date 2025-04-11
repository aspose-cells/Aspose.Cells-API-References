---
title: RadioButtonActiveXControl
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a RadioButton ActiveX control.
type: docs
url: /nodejs-cpp/radiobuttonactivexcontrol/
---

## RadioButtonActiveXControl class

Represents a RadioButton ActiveX control.

```javascript
class RadioButtonActiveXControl extends ToggleButtonActiveXControl;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(ToggleButtonActiveXControl)](#constructor-togglebuttonactivexcontrol-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of the ActiveX control. |
| [getGroupName()](#getGroupName--)| Gets and sets the group's name. |
| [setGroupName(string)](#setGroupName-string-)| Gets and sets the group's name. |
| [getAlignment()](#getAlignment--)| Gets and set the position of the Caption relative to the control. |
| [setAlignment(ControlCaptionAlignmentType)](#setAlignment-controlcaptionalignmenttype-)| Gets and set the position of the Caption relative to the control. |
| [isWordWrapped()](#isWordWrapped--)| Indicates whether the contents of the control automatically wrap at the end of a line. |
| [setIsWordWrapped(boolean)](#setIsWordWrapped-boolean-)| Indicates whether the contents of the control automatically wrap at the end of a line. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getWorkbook()](#getWorkbook--)| Gets the [Workbook](../workbook/) object. |
| [getMouseIcon()](#getMouseIcon--)| Gets and sets a custom icon to display as the mouse pointer for the control. |
| [setMouseIcon(Uint8Array)](#setMouseIcon-uint8array-)| Gets and sets a custom icon to display as the mouse pointer for the control. |
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
| [getCaption()](#getCaption--)| Gets and set the descriptive text that appears on a control. |
| [setCaption(string)](#setCaption-string-)| Gets and set the descriptive text that appears on a control. |
| [getPicturePosition()](#getPicturePosition--)| Gets and set the location of the control's picture relative to its caption. |
| [setPicturePosition(ControlPicturePositionType)](#setPicturePosition-controlpicturepositiontype-)| Gets and set the location of the control's picture relative to its caption. |
| [getSpecialEffect()](#getSpecialEffect--)| Gets and sets the special effect of the control. |
| [setSpecialEffect(ControlSpecialEffectType)](#setSpecialEffect-controlspecialeffecttype-)| Gets and sets the special effect of the control. |
| [getPicture()](#getPicture--)| Gets and sets the data of the picture. |
| [setPicture(Uint8Array)](#setPicture-uint8array-)| Gets and sets the data of the picture. |
| [getAccelerator()](#getAccelerator--)| Gets and sets the accelerator key for the control. |
| [setAccelerator(string)](#setAccelerator-string-)| Gets and sets the accelerator key for the control. |
| [getValue()](#getValue--)| Indicates if the control is checked or not. |
| [setValue(CheckValueType)](#setValue-checkvaluetype-)| Indicates if the control is checked or not. |
| [isTripleState()](#isTripleState--)| Indicates how the specified control will display Null values. |
| [setIsTripleState(boolean)](#setIsTripleState-boolean-)| Indicates how the specified control will display Null values. |
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


### constructor(ToggleButtonActiveXControl) {#constructor-togglebuttonactivexcontrol-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: ToggleButtonActiveXControl);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | ToggleButtonActiveXControl | The parent object. |

### getType() {#getType--}

Gets the type of the ActiveX control.

```javascript
getType() : ControlType;
```


**Returns**

[ControlType](../controltype/)

### getGroupName() {#getGroupName--}

Gets and sets the group's name.

```javascript
getGroupName() : string;
```


### setGroupName(string) {#setGroupName-string-}

Gets and sets the group's name.

```javascript
setGroupName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAlignment() {#getAlignment--}

Gets and set the position of the Caption relative to the control.

```javascript
getAlignment() : ControlCaptionAlignmentType;
```


**Returns**

[ControlCaptionAlignmentType](../controlcaptionalignmenttype/)

### setAlignment(ControlCaptionAlignmentType) {#setAlignment-controlcaptionalignmenttype-}

Gets and set the position of the Caption relative to the control.

```javascript
setAlignment(value: ControlCaptionAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ControlCaptionAlignmentType](../controlcaptionalignmenttype/) | The value to set. |

### isWordWrapped() {#isWordWrapped--}

Indicates whether the contents of the control automatically wrap at the end of a line.

```javascript
isWordWrapped() : boolean;
```


### setIsWordWrapped(boolean) {#setIsWordWrapped-boolean-}

Indicates whether the contents of the control automatically wrap at the end of a line.

```javascript
setIsWordWrapped(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


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
getMouseIcon() : Uint8Array;
```


### setMouseIcon(Uint8Array) {#setMouseIcon-uint8array-}

Gets and sets a custom icon to display as the mouse pointer for the control.

```javascript
setMouseIcon(value: Uint8Array) : void;
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
getData() : Uint8Array;
```


### getCaption() {#getCaption--}

Gets and set the descriptive text that appears on a control.

```javascript
getCaption() : string;
```


### setCaption(string) {#setCaption-string-}

Gets and set the descriptive text that appears on a control.

```javascript
setCaption(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getPicturePosition() {#getPicturePosition--}

Gets and set the location of the control's picture relative to its caption.

```javascript
getPicturePosition() : ControlPicturePositionType;
```


**Returns**

[ControlPicturePositionType](../controlpicturepositiontype/)

### setPicturePosition(ControlPicturePositionType) {#setPicturePosition-controlpicturepositiontype-}

Gets and set the location of the control's picture relative to its caption.

```javascript
setPicturePosition(value: ControlPicturePositionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ControlPicturePositionType](../controlpicturepositiontype/) | The value to set. |

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

### getPicture() {#getPicture--}

Gets and sets the data of the picture.

```javascript
getPicture() : Uint8Array;
```


### setPicture(Uint8Array) {#setPicture-uint8array-}

Gets and sets the data of the picture.

```javascript
setPicture(value: Uint8Array) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### getAccelerator() {#getAccelerator--}

Gets and sets the accelerator key for the control.

```javascript
getAccelerator() : string;
```


### setAccelerator(string) {#setAccelerator-string-}

Gets and sets the accelerator key for the control.

```javascript
setAccelerator(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getValue() {#getValue--}

Indicates if the control is checked or not.

```javascript
getValue() : CheckValueType;
```


**Returns**

[CheckValueType](../checkvaluetype/)

### setValue(CheckValueType) {#setValue-checkvaluetype-}

Indicates if the control is checked or not.

```javascript
setValue(value: CheckValueType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CheckValueType](../checkvaluetype/) | The value to set. |

### isTripleState() {#isTripleState--}

Indicates how the specified control will display Null values.

```javascript
isTripleState() : boolean;
```


**Remarks**

list type="table"> <listheader> <description>Setting</description> <description>Description</description> </listheader> <item> <description>True</description> <description>The control will cycle through states for Yes, No, and Null values. The control appears dimmed (grayed) when its Value property is set to Null.</description> </item> <item> <description>False</description> <description>(Default) The control will cycle through states for Yes and No values. Null values display as if they were No values.</description> </item> </list

### setIsTripleState(boolean) {#setIsTripleState-boolean-}

Indicates how the specified control will display Null values.

```javascript
setIsTripleState(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

list type="table"> <listheader> <description>Setting</description> <description>Description</description> </listheader> <item> <description>True</description> <description>The control will cycle through states for Yes, No, and Null values. The control appears dimmed (grayed) when its Value property is set to Null.</description> </item> <item> <description>False</description> <description>(Default) The control will cycle through states for Yes and No values. Null values display as if they were No values.</description> </item> </list

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


