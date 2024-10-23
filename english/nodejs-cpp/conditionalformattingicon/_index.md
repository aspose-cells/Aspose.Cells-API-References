---
title: ConditionalFormattingIcon
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents  the custom  icon of conditional formatting rule.
type: docs
url: /nodejs-cpp/conditionalformattingicon/
---

## ConditionalFormattingIcon class

Represents  the custom  icon of conditional formatting rule.

```javascript
class ConditionalFormattingIcon;
```


## Methods

| Method | Description |
| --- | --- |
| [getImageData()](#getImageData--)| Gets the icon set data. |
| [getType()](#getType--)| Gets and sets the icon set type. |
| [setType(IconSetType)](#setType-iconsettype-)| Gets and sets the icon set type. |
| [getIndex()](#getIndex--)| Gets and sets the icon's index in the icon set. |
| [setIndex(number)](#setIndex-number-)| Gets and sets the icon's index in the icon set. |
| [getImageData(Cell)](#getImageData-cell-)| Gets the image data with the setting of cell. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| static [getIconImageData(IconSetType, number)](#getIconImageData-iconsettype-number-)| Get the icon set data |


### getImageData() {#getImageData--}

Gets the icon set data.

```javascript
getImageData() : number[];
```


**Returns**

number[]

### getType() {#getType--}

Gets and sets the icon set type.

```javascript
getType() : IconSetType;
```


**Returns**

[IconSetType](../iconsettype/)

### setType(IconSetType) {#setType-iconsettype-}

Gets and sets the icon set type.

```javascript
setType(value: IconSetType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IconSetType](../iconsettype/) | The value to set. |

### getIndex() {#getIndex--}

Gets and sets the icon's index in the icon set.

```javascript
getIndex() : number;
```


### setIndex(number) {#setIndex-number-}

Gets and sets the icon's index in the icon set.

```javascript
setIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getImageData(Cell) {#getImageData-cell-}

Gets the image data with the setting of cell.

```javascript
getImageData(cell: Cell) : number[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [Cell](../cell/) | The setting of cell. |

**Returns**

Returns the image data of icon.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getIconImageData(IconSetType, number) {#getIconImageData-iconsettype-number-}

Get the icon set data

```javascript
static getIconImageData(type: IconSetType, index: number) : number[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [IconSetType](../iconsettype/) | icon's type |
| index | number | icon's index |

**Returns**

number[]


