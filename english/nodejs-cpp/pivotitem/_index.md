---
title: PivotItem
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a item in a PivotField report.
type: docs
url: /nodejs-cpp/pivotitem/
---

## PivotItem class

Represents a item in a PivotField report.

```javascript
class PivotItem;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [isHidden](#isHidden--)| boolean | Gets and Sets whether the pivot item is hidden. |
| [position](#position--)| number | Specifying the position index in all the PivotItems,not the PivotItems under the same parent node. |
| [positionInSameParentNode](#positionInSameParentNode--)| number | Specifying the position index in the PivotItems under the same parent node. |
| [isDetailHidden](#isDetailHidden--)| boolean | Gets and sets whether the detail of this pivot item is hidden. |
| [isCalculatedItem](#isCalculatedItem--)| boolean | Readonly. Indicates whether this pivot item is a calculated formula item. |
| [isMissing](#isMissing--)| boolean | Readonly. Indicates whether the item is removed from the data source. |
| [value](#value--)| Object | Readonly. Gets the value of the pivot item |
| [name](#name--)| string | Gets the name of the pivot item. |
| [index](#index--)| number | Gets the index of the pivot item in cache field. |

## Methods

| Method | Description |
| --- | --- |
| [isHidden()](#isHidden--)| <b>@deprecated.</b> Please use the 'isHidden' property instead. Gets and Sets whether the pivot item is hidden. |
| [setIsHidden(boolean)](#setIsHidden-boolean-)| <b>@deprecated.</b> Please use the 'isHidden' property instead. Gets and Sets whether the pivot item is hidden. |
| [getPosition()](#getPosition--)| <b>@deprecated.</b> Please use the 'position' property instead. Specifying the position index in all the PivotItems,not the PivotItems under the same parent node. |
| [setPosition(number)](#setPosition-number-)| <b>@deprecated.</b> Please use the 'position' property instead. Specifying the position index in all the PivotItems,not the PivotItems under the same parent node. |
| [getPositionInSameParentNode()](#getPositionInSameParentNode--)| <b>@deprecated.</b> Please use the 'positionInSameParentNode' property instead. Specifying the position index in the PivotItems under the same parent node. |
| [setPositionInSameParentNode(number)](#setPositionInSameParentNode-number-)| <b>@deprecated.</b> Please use the 'positionInSameParentNode' property instead. Specifying the position index in the PivotItems under the same parent node. |
| [isDetailHidden()](#isDetailHidden--)| <b>@deprecated.</b> Please use the 'isDetailHidden' property instead. Gets and sets whether the detail of this pivot item is hidden. |
| [setIsDetailHidden(boolean)](#setIsDetailHidden-boolean-)| <b>@deprecated.</b> Please use the 'isDetailHidden' property instead. Gets and sets whether the detail of this pivot item is hidden. |
| [isCalculatedItem()](#isCalculatedItem--)| <b>@deprecated.</b> Please use the 'isCalculatedItem' property instead. Indicates whether this pivot item is a calculated formula item. |
| [isMissing()](#isMissing--)| <b>@deprecated.</b> Please use the 'isMissing' property instead. Indicates whether the item is removed from the data source. |
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Gets the value of the pivot item |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets the name of the pivot item. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Gets the name of the pivot item. |
| [getIndex()](#getIndex--)| <b>@deprecated.</b> Please use the 'index' property instead. Gets the index of the pivot item in cache field. |
| [setIndex(number)](#setIndex-number-)| <b>@deprecated.</b> Please use the 'index' property instead. Gets the index of the pivot item in cache field. |
| [move(number, boolean)](#move-number-boolean-)| Moves the item up or down |
| [getFormula()](#getFormula--)| Gets the formula of this calculated item. Only works when this item is calculated item. |
| [getStringValue()](#getStringValue--)| Gets the string value of the pivot item If the value is null, it will return "" |
| [getDoubleValue()](#getDoubleValue--)| Gets the double value of the pivot item If the value is null or not number ,it will return 0 |
| [getDateTimeValue()](#getDateTimeValue--)| Gets the date time value of the pivot item If the value is null ,it will return DateTime.MinValue |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### isHidden {#isHidden--}

Gets and Sets whether the pivot item is hidden.

```javascript
isHidden : boolean;
```


### position {#position--}

Specifying the position index in all the PivotItems,not the PivotItems under the same parent node.

```javascript
position : number;
```


### positionInSameParentNode {#positionInSameParentNode--}

Specifying the position index in the PivotItems under the same parent node.

```javascript
positionInSameParentNode : number;
```


### isDetailHidden {#isDetailHidden--}

Gets and sets whether the detail of this pivot item is hidden.

```javascript
isDetailHidden : boolean;
```


### isCalculatedItem {#isCalculatedItem--}

Readonly. Indicates whether this pivot item is a calculated formula item.

```javascript
isCalculatedItem : boolean;
```


### isMissing {#isMissing--}

Readonly. Indicates whether the item is removed from the data source.

```javascript
isMissing : boolean;
```


**Remarks**

True means this value has been removed from the data source.

### value {#value--}

Readonly. Gets the value of the pivot item

```javascript
value : Object;
```


### name {#name--}

Gets the name of the pivot item.

```javascript
name : string;
```


### index {#index--}

Gets the index of the pivot item in cache field.

```javascript
index : number;
```


### isHidden() {#isHidden--}

<b>@deprecated.</b> Please use the 'isHidden' property instead. Gets and Sets whether the pivot item is hidden.

```javascript
isHidden() : boolean;
```


### setIsHidden(boolean) {#setIsHidden-boolean-}

<b>@deprecated.</b> Please use the 'isHidden' property instead. Gets and Sets whether the pivot item is hidden.

```javascript
setIsHidden(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPosition() {#getPosition--}

<b>@deprecated.</b> Please use the 'position' property instead. Specifying the position index in all the PivotItems,not the PivotItems under the same parent node.

```javascript
getPosition() : number;
```


### setPosition(number) {#setPosition-number-}

<b>@deprecated.</b> Please use the 'position' property instead. Specifying the position index in all the PivotItems,not the PivotItems under the same parent node.

```javascript
setPosition(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getPositionInSameParentNode() {#getPositionInSameParentNode--}

<b>@deprecated.</b> Please use the 'positionInSameParentNode' property instead. Specifying the position index in the PivotItems under the same parent node.

```javascript
getPositionInSameParentNode() : number;
```


### setPositionInSameParentNode(number) {#setPositionInSameParentNode-number-}

<b>@deprecated.</b> Please use the 'positionInSameParentNode' property instead. Specifying the position index in the PivotItems under the same parent node.

```javascript
setPositionInSameParentNode(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isDetailHidden() {#isDetailHidden--}

<b>@deprecated.</b> Please use the 'isDetailHidden' property instead. Gets and sets whether the detail of this pivot item is hidden.

```javascript
isDetailHidden() : boolean;
```


### setIsDetailHidden(boolean) {#setIsDetailHidden-boolean-}

<b>@deprecated.</b> Please use the 'isDetailHidden' property instead. Gets and sets whether the detail of this pivot item is hidden.

```javascript
setIsDetailHidden(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isCalculatedItem() {#isCalculatedItem--}

<b>@deprecated.</b> Please use the 'isCalculatedItem' property instead. Indicates whether this pivot item is a calculated formula item.

```javascript
isCalculatedItem() : boolean;
```


### isMissing() {#isMissing--}

<b>@deprecated.</b> Please use the 'isMissing' property instead. Indicates whether the item is removed from the data source.

```javascript
isMissing() : boolean;
```


**Remarks**

True means this value has been removed from the data source.

### getValue() {#getValue--}

<b>@deprecated.</b> Please use the 'value' property instead. Gets the value of the pivot item

```javascript
getValue() : Object;
```


### getName() {#getName--}

<b>@deprecated.</b> Please use the 'name' property instead. Gets the name of the pivot item.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

<b>@deprecated.</b> Please use the 'name' property instead. Gets the name of the pivot item.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getIndex() {#getIndex--}

<b>@deprecated.</b> Please use the 'index' property instead. Gets the index of the pivot item in cache field.

```javascript
getIndex() : number;
```


### setIndex(number) {#setIndex-number-}

<b>@deprecated.</b> Please use the 'index' property instead. Gets the index of the pivot item in cache field.

```javascript
setIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### move(number, boolean) {#move-number-boolean-}

Moves the item up or down

```javascript
move(count: number, isSameParent: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| count | number | The number of moving up or down.         /// Move the item up if this is less than zero;         /// Move the item down if this is greater than zero. |
| isSameParent | boolean | Specifying whether moving operation is in the same parent node or not |

### getFormula() {#getFormula--}

Gets the formula of this calculated item. Only works when this item is calculated item.

```javascript
getFormula() : string;
```


### getStringValue() {#getStringValue--}

Gets the string value of the pivot item If the value is null, it will return ""

```javascript
getStringValue() : string;
```


### getDoubleValue() {#getDoubleValue--}

Gets the double value of the pivot item If the value is null or not number ,it will return 0

```javascript
getDoubleValue() : number;
```


### getDateTimeValue() {#getDateTimeValue--}

Gets the date time value of the pivot item If the value is null ,it will return DateTime.MinValue

```javascript
getDateTimeValue() : Date;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



