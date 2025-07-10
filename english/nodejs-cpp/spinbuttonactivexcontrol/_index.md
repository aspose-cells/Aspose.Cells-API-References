﻿---
title: SpinButtonActiveXControl
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the SpinButton control.
type: docs
url: /nodejs-cpp/spinbuttonactivexcontrol/
---

## SpinButtonActiveXControl class

Represents the SpinButton control.

```javascript
class SpinButtonActiveXControl extends ActiveXControl;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor(ActiveXControl)](#constructor-activexcontrol-)| Constructs from a parent object convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [min](#min--)| number | Gets and sets the minimum acceptable value. |
| [max](#max--)| number | Gets and sets the maximum acceptable value. |
| [position](#position--)| number | Gets and sets the value. |
| [smallChange](#smallChange--)| number | Gets and sets the amount by which the Position property changes |
| [orientation](#orientation--)| ControlScrollOrientation | Gets and sets whether the SpinButton or ScrollBar is oriented vertically or horizontally. |
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
| [getMin()](#getMin--)| <b>@deprecated.</b> Please use the 'min' property instead. Gets and sets the minimum acceptable value. |
| [setMin(number)](#setMin-number-)| <b>@deprecated.</b> Please use the 'min' property instead. Gets and sets the minimum acceptable value. |
| [getMax()](#getMax--)| <b>@deprecated.</b> Please use the 'max' property instead. Gets and sets the maximum acceptable value. |
| [setMax(number)](#setMax-number-)| <b>@deprecated.</b> Please use the 'max' property instead. Gets and sets the maximum acceptable value. |
| [getPosition()](#getPosition--)| <b>@deprecated.</b> Please use the 'position' property instead. Gets and sets the value. |
| [setPosition(number)](#setPosition-number-)| <b>@deprecated.</b> Please use the 'position' property instead. Gets and sets the value. |
| [getSmallChange()](#getSmallChange--)| <b>@deprecated.</b> Please use the 'smallChange' property instead. Gets and sets the amount by which the Position property changes |
| [setSmallChange(number)](#setSmallChange-number-)| <b>@deprecated.</b> Please use the 'smallChange' property instead. Gets and sets the amount by which the Position property changes |
| [getOrientation()](#getOrientation--)| <b>@deprecated.</b> Please use the 'orientation' property instead. Gets and sets whether the SpinButton or ScrollBar is oriented vertically or horizontally. |
| [setOrientation(ControlScrollOrientation)](#setOrientation-controlscrollorientation-)| <b>@deprecated.</b> Please use the 'orientation' property instead. Gets and sets whether the SpinButton or ScrollBar is oriented vertically or horizontally. |
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

### min {#min--}

Gets and sets the minimum acceptable value.

```javascript
min : number;
```


### max {#max--}

Gets and sets the maximum acceptable value.

```javascript
max : number;
```


### position {#position--}

Gets and sets the value.

```javascript
position : number;
```


### smallChange {#smallChange--}

Gets and sets the amount by which the Position property changes

```javascript
smallChange : number;
```


### orientation {#orientation--}

Gets and sets whether the SpinButton or ScrollBar is oriented vertically or horizontally.

```javascript
orientation : ControlScrollOrientation;
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


### getMin() {#getMin--}

<b>@deprecated.</b> Please use the 'min' property instead. Gets and sets the minimum acceptable value.

```javascript
getMin() : number;
```


### setMin(number) {#setMin-number-}

<b>@deprecated.</b> Please use the 'min' property instead. Gets and sets the minimum acceptable value.

```javascript
setMin(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getMax() {#getMax--}

<b>@deprecated.</b> Please use the 'max' property instead. Gets and sets the maximum acceptable value.

```javascript
getMax() : number;
```


### setMax(number) {#setMax-number-}

<b>@deprecated.</b> Please use the 'max' property instead. Gets and sets the maximum acceptable value.

```javascript
setMax(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getPosition() {#getPosition--}

<b>@deprecated.</b> Please use the 'position' property instead. Gets and sets the value.

```javascript
getPosition() : number;
```


### setPosition(number) {#setPosition-number-}

<b>@deprecated.</b> Please use the 'position' property instead. Gets and sets the value.

```javascript
setPosition(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getSmallChange() {#getSmallChange--}

<b>@deprecated.</b> Please use the 'smallChange' property instead. Gets and sets the amount by which the Position property changes

```javascript
getSmallChange() : number;
```


### setSmallChange(number) {#setSmallChange-number-}

<b>@deprecated.</b> Please use the 'smallChange' property instead. Gets and sets the amount by which the Position property changes

```javascript
setSmallChange(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getOrientation() {#getOrientation--}

<b>@deprecated.</b> Please use the 'orientation' property instead. Gets and sets whether the SpinButton or ScrollBar is oriented vertically or horizontally.

```javascript
getOrientation() : ControlScrollOrientation;
```


**Returns**

[ControlScrollOrientation](../controlscrollorientation/)

### setOrientation(ControlScrollOrientation) {#setOrientation-controlscrollorientation-}

<b>@deprecated.</b> Please use the 'orientation' property instead. Gets and sets whether the SpinButton or ScrollBar is oriented vertically or horizontally.

```javascript
setOrientation(value: ControlScrollOrientation) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ControlScrollOrientation](../controlscrollorientation/) | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getWorkbook() {#getWorkbook--}

<b>@deprecated.</b> Please use the 'workbook' property instead. Gets the [Workbook](../workbook/) object.

```javascript
getWorkbook() : Workbook;
```


**Returns**

[Workbook](../workbook/)

### getMouseIcon() {#getMouseIcon--}

<b>@deprecated.</b> Please use the 'mouseIcon' property instead. Gets and sets a custom icon to display as the mouse pointer for the control.

```javascript
getMouseIcon() : Uint8Array;
```


### setMouseIcon(Uint8Array) {#setMouseIcon-uint8array-}

<b>@deprecated.</b> Please use the 'mouseIcon' property instead. Gets and sets a custom icon to display as the mouse pointer for the control.

```javascript
setMouseIcon(value: Uint8Array) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### getMousePointer() {#getMousePointer--}

<b>@deprecated.</b> Please use the 'mousePointer' property instead. Gets and sets the type of icon displayed as the mouse pointer for the control.

```javascript
getMousePointer() : ControlMousePointerType;
```


**Returns**

[ControlMousePointerType](../controlmousepointertype/)

### setMousePointer(ControlMousePointerType) {#setMousePointer-controlmousepointertype-}

<b>@deprecated.</b> Please use the 'mousePointer' property instead. Gets and sets the type of icon displayed as the mouse pointer for the control.

```javascript
setMousePointer(value: ControlMousePointerType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ControlMousePointerType](../controlmousepointertype/) | The value to set. |

### getLinkedCell() {#getLinkedCell--}

<b>@deprecated.</b> Please use the 'linkedCell' property instead. Gets and sets the linked cell.

```javascript
getLinkedCell() : string;
```


### setLinkedCell(string) {#setLinkedCell-string-}

<b>@deprecated.</b> Please use the 'linkedCell' property instead. Gets and sets the linked cell.

```javascript
setLinkedCell(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getListFillRange() {#getListFillRange--}

<b>@deprecated.</b> Please use the 'listFillRange' property instead. Gets and sets the list fill range.

```javascript
getListFillRange() : string;
```


### setListFillRange(string) {#setListFillRange-string-}

<b>@deprecated.</b> Please use the 'listFillRange' property instead. Gets and sets the list fill range.

```javascript
setListFillRange(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isEnabled() {#isEnabled--}

<b>@deprecated.</b> Please use the 'isEnabled' property instead. Indicates whether the control can receive the focus and respond to user-generated events.

```javascript
isEnabled() : boolean;
```


### setIsEnabled(boolean) {#setIsEnabled-boolean-}

<b>@deprecated.</b> Please use the 'isEnabled' property instead. Indicates whether the control can receive the focus and respond to user-generated events.

```javascript
setIsEnabled(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isLocked() {#isLocked--}

<b>@deprecated.</b> Please use the 'isLocked' property instead. Indicates whether data in the control is locked for editing.

```javascript
isLocked() : boolean;
```


### setIsLocked(boolean) {#setIsLocked-boolean-}

<b>@deprecated.</b> Please use the 'isLocked' property instead. Indicates whether data in the control is locked for editing.

```javascript
setIsLocked(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isTransparent() {#isTransparent--}

<b>@deprecated.</b> Please use the 'isTransparent' property instead. Indicates whether the control is transparent.

```javascript
isTransparent() : boolean;
```


### setIsTransparent(boolean) {#setIsTransparent-boolean-}

<b>@deprecated.</b> Please use the 'isTransparent' property instead. Indicates whether the control is transparent.

```javascript
setIsTransparent(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getIMEMode() {#getIMEMode--}

<b>@deprecated.</b> Please use the 'iMEMode' property instead. Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus.

```javascript
getIMEMode() : InputMethodEditorMode;
```


**Returns**

[InputMethodEditorMode](../inputmethodeditormode/)

### setIMEMode(InputMethodEditorMode) {#setIMEMode-inputmethodeditormode-}

<b>@deprecated.</b> Please use the 'iMEMode' property instead. Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus.

```javascript
setIMEMode(value: InputMethodEditorMode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [InputMethodEditorMode](../inputmethodeditormode/) | The value to set. |

### getFont() {#getFont--}

<b>@deprecated.</b> Please use the 'font' property instead. Represents the font of the control.

```javascript
getFont() : Font;
```


**Returns**

[Font](../font/)

### getTextAlign() {#getTextAlign--}

<b>@deprecated.</b> Please use the 'textAlign' property instead. Represents how to align the text used by the control.

```javascript
getTextAlign() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](../textalignmenttype/)

### setTextAlign(TextAlignmentType) {#setTextAlign-textalignmenttype-}

<b>@deprecated.</b> Please use the 'textAlign' property instead. Represents how to align the text used by the control.

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



