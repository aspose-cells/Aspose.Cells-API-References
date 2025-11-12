---
title: ColorFilter
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents setting for filtering the range by color.
type: docs
url: /javascript-cpp/colorfilter/
---

## ColorFilter class

Represents setting for filtering the range by color.

```javascript
class ColorFilter;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(VObject)](#constructor-vobject-)| Constructs from a VObject convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [filterByFillColor](#filterByFillColor--)| boolean | Whether filter by the cell's fill color. |

## Methods

| Method | Description |
| --- | --- |
| [getColor(WorksheetCollection)](#getColor-worksheetcollection-)| Gets the color of this filter. |
| [toVObject()](#toVObject--)| Gets the VObject. |


### constructor(VObject) {#constructor-vobject-}

Constructs from a VObject convertible to this.

```javascript
constructor(vobj: VObject);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vobj | VObject | The vobject. |

### filterByFillColor {#filterByFillColor--}

Whether filter by the cell's fill color.

```javascript
filterByFillColor : boolean;
```


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

### toVObject() {#toVObject--}

Gets the VObject.

```javascript
toVObject() : VObject;
```



