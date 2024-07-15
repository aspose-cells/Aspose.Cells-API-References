---
title: PivotArea
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Presents the selected area of the PivotTable.
type: docs
url: /nodejs-cpp/pivotarea/
---

## PivotArea class

Presents the selected area of the PivotTable.

```javascript
class PivotArea;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(PivotTable)](#constructor-pivottable-)| Presents the selected area of the PivotTable. |

## Methods

| Method | Description |
| --- | --- |
| [getFilters()](#getFilters--)| Gets all filters for this PivotArea. |
| [getOnlyData()](#getOnlyData--)| Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels. |
| [setOnlyData(boolean)](#setOnlyData-boolean-)| Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels. |
| [getOnlyLabel()](#getOnlyLabel--)| Indicates whether only the data labels for an item selection are selected. |
| [setOnlyLabel(boolean)](#setOnlyLabel-boolean-)| Indicates whether only the data labels for an item selection are selected. |
| [isRowGrandIncluded()](#isRowGrandIncluded--)| Indicates whether the row grand total is included. |
| [setIsRowGrandIncluded(boolean)](#setIsRowGrandIncluded-boolean-)| Indicates whether the row grand total is included. |
| [isColumnGrandIncluded()](#isColumnGrandIncluded--)| Indicates whether the column grand total is included. |
| [setIsColumnGrandIncluded(boolean)](#setIsColumnGrandIncluded-boolean-)| Indicates whether the column grand total is included. |
| [getAxisType()](#getAxisType--)| Gets and sets the region of the PivotTable to which this rule applies. |
| [setAxisType(PivotFieldType)](#setAxisType-pivotfieldtype-)| Gets and sets the region of the PivotTable to which this rule applies. |
| [getRuleType()](#getRuleType--)| Gets and sets the type of selection rule. |
| [setRuleType(PivotAreaType)](#setRuleType-pivotareatype-)| Gets and sets the type of selection rule. |
| [isOutline()](#isOutline--)| Indicates whether the rule refers to an area that is in outline mode. |
| [setIsOutline(boolean)](#setIsOutline-boolean-)| Indicates whether the rule refers to an area that is in outline mode. |
| [select(PivotFieldType, number, PivotTableSelectionType)](#select-pivotfieldtype-number-pivottableselectiontype-)| Select the area with filters. |


### constructor(PivotTable) {#constructor-pivottable-}

Presents the selected area of the PivotTable.

```javascript
constructor(table: PivotTable);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| table | [PivotTable](../pivottable/) |  |

### getFilters() {#getFilters--}

Gets all filters for this PivotArea.

```javascript
getFilters() : PivotAreaFilterCollection;
```


**Returns**

[PivotAreaFilterCollection](../pivotareafiltercollection/)

### getOnlyData() {#getOnlyData--}

Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels.

```javascript
getOnlyData() : boolean;
```


### setOnlyData(boolean) {#setOnlyData-boolean-}

Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels.

```javascript
setOnlyData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getOnlyLabel() {#getOnlyLabel--}

Indicates whether only the data labels for an item selection are selected.

```javascript
getOnlyLabel() : boolean;
```


### setOnlyLabel(boolean) {#setOnlyLabel-boolean-}

Indicates whether only the data labels for an item selection are selected.

```javascript
setOnlyLabel(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isRowGrandIncluded() {#isRowGrandIncluded--}

Indicates whether the row grand total is included.

```javascript
isRowGrandIncluded() : boolean;
```


### setIsRowGrandIncluded(boolean) {#setIsRowGrandIncluded-boolean-}

Indicates whether the row grand total is included.

```javascript
setIsRowGrandIncluded(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isColumnGrandIncluded() {#isColumnGrandIncluded--}

Indicates whether the column grand total is included.

```javascript
isColumnGrandIncluded() : boolean;
```


### setIsColumnGrandIncluded(boolean) {#setIsColumnGrandIncluded-boolean-}

Indicates whether the column grand total is included.

```javascript
setIsColumnGrandIncluded(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAxisType() {#getAxisType--}

Gets and sets the region of the PivotTable to which this rule applies.

```javascript
getAxisType() : PivotFieldType;
```


**Returns**

[PivotFieldType](../pivotfieldtype/)

### setAxisType(PivotFieldType) {#setAxisType-pivotfieldtype-}

Gets and sets the region of the PivotTable to which this rule applies.

```javascript
setAxisType(value: PivotFieldType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotFieldType](../pivotfieldtype/) | The value to set. |

### getRuleType() {#getRuleType--}

Gets and sets the type of selection rule.

```javascript
getRuleType() : PivotAreaType;
```


**Returns**

[PivotAreaType](../pivotareatype/)

### setRuleType(PivotAreaType) {#setRuleType-pivotareatype-}

Gets and sets the type of selection rule.

```javascript
setRuleType(value: PivotAreaType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotAreaType](../pivotareatype/) | The value to set. |

### isOutline() {#isOutline--}

Indicates whether the rule refers to an area that is in outline mode.

```javascript
isOutline() : boolean;
```


### setIsOutline(boolean) {#setIsOutline-boolean-}

Indicates whether the rule refers to an area that is in outline mode.

```javascript
setIsOutline(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### select(PivotFieldType, number, PivotTableSelectionType) {#select-pivotfieldtype-number-pivottableselectiontype-}

Select the area with filters.

```javascript
select(axisType: PivotFieldType, fieldPosition: number, selectionType: PivotTableSelectionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | [PivotFieldType](../pivotfieldtype/) | The region of the PivotTable to which this rule applies. |
| fieldPosition | number | Position of the field within the axis to which this rule applies. |
| selectionType | [PivotTableSelectionType](../pivottableselectiontype/) | Specifies what can be selected in a PivotTable during a structured selection. |


