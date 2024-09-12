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


## Methods

| Method | Description |
| --- | --- |
| [isHidden()](#isHidden--)| Gets and Sets whether the pivot item is hidden. |
| [setIsHidden(boolean)](#setIsHidden-boolean-)| Gets and Sets whether the pivot item is hidden. |
| [getPosition()](#getPosition--)| Specifying the position index in all the PivotItems,not the PivotItems under the same parent node. |
| [setPosition(number)](#setPosition-number-)| Specifying the position index in all the PivotItems,not the PivotItems under the same parent node. |
| [getPositionInSameParentNode()](#getPositionInSameParentNode--)| Specifying the position index in the PivotItems under the same parent node. |
| [setPositionInSameParentNode(number)](#setPositionInSameParentNode-number-)| Specifying the position index in the PivotItems under the same parent node. |
| [isHideDetail()](#isHideDetail--)| Gets and Sets whether the pivot item hides detail. |
| [setIsHideDetail(boolean)](#setIsHideDetail-boolean-)| Gets and Sets whether the pivot item hides detail. |
| [isFormula()](#isFormula--)| Indicates whether this pivot item is a calculated formula item. |
| [setIsFormula(boolean)](#setIsFormula-boolean-)| Indicates whether this pivot item is a calculated formula item. |
| [isMissing()](#isMissing--)| Indicates whether the item is removed from the data source. |
| [getValue()](#getValue--)| Gets the value of the pivot item |
| [getName()](#getName--)| Gets the name of the pivot item. |
| [setName(string)](#setName-string-)| Gets the name of the pivot item. |
| [getIndex()](#getIndex--)| Gets the index of the pivot item in cache field. |
| [setIndex(number)](#setIndex-number-)| Gets the index of the pivot item in cache field. |
| [move(number, boolean)](#move-number-boolean-)| Moves the item up or down |
| [getFormula()](#getFormula--)| Gets the formula of this calculated item. Only works when this item is calculated item. |
| [getStringValue()](#getStringValue--)| Gets the string value of the pivot item If the value is null, it will return "" |
| [getDoubleValue()](#getDoubleValue--)| Gets the double value of the pivot item If the value is null or not number ,it will return 0 |
| [getDateTimeValue()](#getDateTimeValue--)| Gets the date time value of the pivot item If the value is null ,it will return DateTime.MinValue |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### isHidden() {#isHidden--}

Gets and Sets whether the pivot item is hidden.

```javascript
isHidden() : boolean;
```


### setIsHidden(boolean) {#setIsHidden-boolean-}

Gets and Sets whether the pivot item is hidden.

```javascript
setIsHidden(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPosition() {#getPosition--}

Specifying the position index in all the PivotItems,not the PivotItems under the same parent node.

```javascript
getPosition() : number;
```


### setPosition(number) {#setPosition-number-}

Specifying the position index in all the PivotItems,not the PivotItems under the same parent node.

```javascript
setPosition(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getPositionInSameParentNode() {#getPositionInSameParentNode--}

Specifying the position index in the PivotItems under the same parent node.

```javascript
getPositionInSameParentNode() : number;
```


### setPositionInSameParentNode(number) {#setPositionInSameParentNode-number-}

Specifying the position index in the PivotItems under the same parent node.

```javascript
setPositionInSameParentNode(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isHideDetail() {#isHideDetail--}

Gets and Sets whether the pivot item hides detail.

```javascript
isHideDetail() : boolean;
```


### setIsHideDetail(boolean) {#setIsHideDetail-boolean-}

Gets and Sets whether the pivot item hides detail.

```javascript
setIsHideDetail(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isFormula() {#isFormula--}

Indicates whether this pivot item is a calculated formula item.

```javascript
isFormula() : boolean;
```


### setIsFormula(boolean) {#setIsFormula-boolean-}

Indicates whether this pivot item is a calculated formula item.

```javascript
setIsFormula(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isMissing() {#isMissing--}

Indicates whether the item is removed from the data source.

```javascript
isMissing() : boolean;
```


**Remarks**

True means this value has benn removed from the data source.

### getValue() {#getValue--}

Gets the value of the pivot item

```javascript
getValue() : object;
```


### getName() {#getName--}

Gets the name of the pivot item.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Gets the name of the pivot item.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getIndex() {#getIndex--}

Gets the index of the pivot item in cache field.

```javascript
getIndex() : number;
```


### setIndex(number) {#setIndex-number-}

Gets the index of the pivot item in cache field.

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



