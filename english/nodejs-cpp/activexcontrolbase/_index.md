---
title: ActiveXControlBase
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the ActiveX control.
type: docs
url: /nodejs-cpp/activexcontrolbase/
---

## ActiveXControlBase class

Represents the ActiveX control.

```javascript
class ActiveXControlBase;
```


## Methods

| Method | Description |
| --- | --- |
| [getWorkbook()](#getWorkbook--)| Gets the [Workbook](../workbook/) object. |
| [getMouseIcon()](#getMouseIcon--)| Gets and sets a custom icon to display as the mouse pointer for the control. |
| [setMouseIcon(Uint8Array)](#setMouseIcon-uint8array-)| Gets and sets a custom icon to display as the mouse pointer for the control. |
| [getMousePointer()](#getMousePointer--)| Gets and sets the type of icon displayed as the mouse pointer for the control. |
| [setMousePointer(ControlMousePointerType)](#setMousePointer-controlmousepointertype-)| Gets and sets the type of icon displayed as the mouse pointer for the control. |
| [getLinkedCell()](#getLinkedCell--)| Gets and sets the linked cell. |
| [setLinkedCell(string)](#setLinkedCell-string-)| Gets and sets the linked cell. |
| [getListFillRange()](#getListFillRange--)| Gets and sets the list fill range. |
| [setListFillRange(string)](#setListFillRange-string-)| Gets and sets the list fill range. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
| [getData()](#getData--)| Gets and sets the binary data of the control. |


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

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


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

### getData() {#getData--}

Gets and sets the binary data of the control.

```javascript
getData() : Uint8Array;
```



