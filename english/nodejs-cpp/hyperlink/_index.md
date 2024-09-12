---
title: Hyperlink
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents a hyperlink.
type: docs
url: /nodejs-cpp/hyperlink/
---

## Hyperlink class

Encapsulates the object that represents a hyperlink.

```javascript
class Hyperlink;
```


## Methods

| Method | Description |
| --- | --- |
| [getAddress()](#getAddress--)| Represents the address of a hyperlink. |
| [setAddress(string)](#setAddress-string-)| Represents the address of a hyperlink. |
| [getTextToDisplay()](#getTextToDisplay--)| Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink. |
| [setTextToDisplay(string)](#setTextToDisplay-string-)| Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink. |
| [getArea()](#getArea--)| Gets the range of hyperlink. |
| [getScreenTip()](#getScreenTip--)| Returns or sets the ScreenTip text for the specified hyperlink. |
| [setScreenTip(string)](#setScreenTip-string-)| Returns or sets the ScreenTip text for the specified hyperlink. |
| [getLinkType()](#getLinkType--)| Gets the link type. |
| [delete()](#delete--)| Deletes this hyperlink |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getAddress() {#getAddress--}

Represents the address of a hyperlink.

```javascript
getAddress() : string;
```


### setAddress(string) {#setAddress-string-}

Represents the address of a hyperlink.

```javascript
setAddress(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTextToDisplay() {#getTextToDisplay--}

Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink.

```javascript
getTextToDisplay() : string;
```


### setTextToDisplay(string) {#setTextToDisplay-string-}

Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink.

```javascript
setTextToDisplay(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getArea() {#getArea--}

Gets the range of hyperlink.

```javascript
getArea() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### getScreenTip() {#getScreenTip--}

Returns or sets the ScreenTip text for the specified hyperlink.

```javascript
getScreenTip() : string;
```


### setScreenTip(string) {#setScreenTip-string-}

Returns or sets the ScreenTip text for the specified hyperlink.

```javascript
setScreenTip(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getLinkType() {#getLinkType--}

Gets the link type.

```javascript
getLinkType() : TargetModeType;
```


**Returns**

[TargetModeType](../targetmodetype/)

### delete() {#delete--}

Deletes this hyperlink

```javascript
delete() : void;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



