---
title: TableStyleElement
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the element of the table style.
type: docs
url: /nodejs-cpp/tablestyleelement/
---

## TableStyleElement class

Represents the element of the table style.

```javascript
class TableStyleElement;
```


## Methods

| Method | Description |
| --- | --- |
| [getSize()](#getSize--)| Number of rows or columns in a single band of striping. Applies only when type is firstRowStripe, secondRowStripe, firstColumnStripe, or secondColumnStripe. |
| [setSize(number)](#setSize-number-)| Number of rows or columns in a single band of striping. Applies only when type is firstRowStripe, secondRowStripe, firstColumnStripe, or secondColumnStripe. |
| [getType()](#getType--)| Gets the element type. |
| [getElementStyle()](#getElementStyle--)| Gets the element style. |
| [setElementStyle(Style)](#setElementStyle-style-)| Sets the element style. |


### getSize() {#getSize--}

Number of rows or columns in a single band of striping. Applies only when type is firstRowStripe, secondRowStripe, firstColumnStripe, or secondColumnStripe.

```javascript
getSize() : number;
```


### setSize(number) {#setSize-number-}

Number of rows or columns in a single band of striping. Applies only when type is firstRowStripe, secondRowStripe, firstColumnStripe, or secondColumnStripe.

```javascript
setSize(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getType() {#getType--}

Gets the element type.

```javascript
getType() : TableStyleElementType;
```


**Returns**

[TableStyleElementType](./tablestyleelementtype/)

### getElementStyle() {#getElementStyle--}

Gets the element style.

```javascript
getElementStyle() : Style;
```


**Returns**

Returns the [Style](./style/) object.

### setElementStyle(Style) {#setElementStyle-style-}

Sets the element style.

```javascript
setElementStyle(style: Style) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](./style/) | The element style. |


