---
title: ColorFilter
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents filtering the range by color.
type: docs
url: /nodejs-cpp/colorfilter/
---

## ColorFilter class

Represents filtering the range by color.

```javascript
class ColorFilter;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(IObject)](#constructor-iobject-)| Constructs from an IObject convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getFilterByFillColor()](#getFilterByFillColor--)| Whether filter by the cell's fill color. |
| [setFilterByFillColor(boolean)](#setFilterByFillColor-boolean-)| Whether filter by the cell's fill color. |
| [getColor(WorksheetCollection)](#getColor-worksheetcollection-)| Gets the color of this filter. |


### constructor(IObject) {#constructor-iobject-}

Constructs from an IObject convertible to this.

```javascript
constructor(obj: IObject);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | IObject | The object. |

### getFilterByFillColor() {#getFilterByFillColor--}

Whether filter by the cell's fill color.

```javascript
getFilterByFillColor() : boolean;
```


**Remarks**

True: cell's fill color; False: cell's font color.

### setFilterByFillColor(boolean) {#setFilterByFillColor-boolean-}

Whether filter by the cell's fill color.

```javascript
setFilterByFillColor(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

True: cell's fill color; False: cell's font color.

### getColor(WorksheetCollection) {#getColor-worksheetcollection-}

Gets the color of this filter.

```javascript
getColor(sheets: WorksheetCollection) : Color;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheets | [WorksheetCollection](../worksheetcollection/) |  |

**Returns**

[Color](../color/)


