---
title: FormatConditionCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents conditional formatting. The FormatConditions can contain up to three conditional formats.
type: docs
url: /nodejs-cpp/formatconditioncollection/
---

## FormatConditionCollection class

Represents conditional formatting. The FormatConditions can contain up to three conditional formats.

```javascript
class FormatConditionCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the formatting condition by index. |
| [getCount()](#getCount--)| Gets the count of the conditions. |
| [getRangeCount()](#getRangeCount--)| Gets count of conditionally formatted ranges. |
| [add(CellArea, FormatConditionType, OperatorType, string, string)](#add-cellarea-formatconditiontype-operatortype-string-string-)| Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting. |
| [addArea(CellArea)](#addArea-cellarea-)| Adds a conditional formatted cell range. |
| [addCondition(FormatConditionType, OperatorType, string, string)](#addCondition-formatconditiontype-operatortype-string-string-)| Adds a formatting condition. |
| [addCondition(FormatConditionType)](#addCondition-formatconditiontype-)| Add a format condition. |
| [getCellArea(number)](#getCellArea-number-)| Gets the conditional formatted cell range by index. |
| [removeArea(number)](#removeArea-number-)| Removes conditional formatted cell range by index. |
| [removeArea(number, number, number, number)](#removeArea-number-number-number-number-)| Remove conditional formatting int the range. |
| [removeCondition(number)](#removeCondition-number-)| Removes the formatting condition by index. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number) {#get-number-}

Gets the formatting condition by index.

```javascript
get(index: number) : FormatCondition;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | the index of the formatting condition to return. |

**Returns**

the formatting condition

### getCount() {#getCount--}

Gets the count of the conditions.

```javascript
getCount() : number;
```


### getRangeCount() {#getRangeCount--}

Gets count of conditionally formatted ranges.

```javascript
getRangeCount() : number;
```


### add(CellArea, FormatConditionType, OperatorType, string, string) {#add-cellarea-formatconditiontype-operatortype-string-string-}

Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting.

```javascript
add(cellArea: CellArea, type: FormatConditionType, operatorType: OperatorType, formula1: string, formula2: string) : number[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../cellarea/) | Conditional formatted cell range. |
| type | [FormatConditionType](../formatconditiontype/) | Type of conditional formatting.It could be one of the members of FormatConditionType. |
| operatorType | [OperatorType](../operatortype/) | Comparison operator.It could be one of the members of OperatorType. |
| formula1 | string | The value or expression associated with conditional formatting. |
| formula2 | string | The value or expression associated with conditional formatting |

**Returns**

[0]:Formatting condition object index;[1] Effected cell rang index.

### addArea(CellArea) {#addArea-cellarea-}

Adds a conditional formatted cell range.

```javascript
addArea(cellArea: CellArea) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../cellarea/) | Conditional formatted cell range. |

**Returns**

Conditional formatted cell rang index.

### addCondition(FormatConditionType, OperatorType, string, string) {#addCondition-formatconditiontype-operatortype-string-string-}

Adds a formatting condition.

```javascript
addCondition(type: FormatConditionType, operatorType: OperatorType, formula1: string, formula2: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [FormatConditionType](../formatconditiontype/) | The type of format condition. |
| operatorType | [OperatorType](../operatortype/) | The operator type |
| formula1 | string | The value or expression associated with conditional formatting.         /// If the input value starts with '=', then it will be taken as formula.         /// Otherwise it will be taken as plain value(text, number, bool).         /// For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | string | The value or expression associated with conditional formatting.         /// The input format is same with formula1 |

**Returns**

Formatting condition object index;

### addCondition(FormatConditionType) {#addCondition-formatconditiontype-}

Add a format condition.

```javascript
addCondition(type: FormatConditionType) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [FormatConditionType](../formatconditiontype/) | Format condition type. |

**Returns**

Formatting condition object index;

### getCellArea(number) {#getCellArea-number-}

Gets the conditional formatted cell range by index.

```javascript
getCellArea(index: number) : CellArea;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | the index of the conditional formatted cell range. |

**Returns**

the conditional formatted cell range

### removeArea(number) {#removeArea-number-}

Removes conditional formatted cell range by index.

```javascript
removeArea(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index of the conditional formatted cell range to be removed. |

### removeArea(number, number, number, number) {#removeArea-number-number-number-number-}

Remove conditional formatting int the range.

```javascript
removeArea(startRow: number, startColumn: number, totalRows: number, totalColumns: number) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | The startRow of the range. |
| startColumn | number | The startColumn of the range. |
| totalRows | number | The number of rows of the range. |
| totalColumns | number | The number of columns of the range. |

**Returns**

Returns TRUE, this FormatCondtionCollection should be removed.

### removeCondition(number) {#removeCondition-number-}

Removes the formatting condition by index.

```javascript
removeCondition(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index of the formatting condition to be removed. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



