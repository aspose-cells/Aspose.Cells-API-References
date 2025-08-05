﻿---
title: PivotArea
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Presents the selected area of the PivotTable.
type: docs
url: /js-cpp/pivotarea/
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

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [filters](#filters--)| PivotAreaFilterCollection | Readonly. Gets all filters for this PivotArea. |
| [onlyData](#onlyData--)| boolean | Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels. |
| [onlyLabel](#onlyLabel--)| boolean | Indicates whether only the data labels for an item selection are selected. |
| [isRowGrandIncluded](#isRowGrandIncluded--)| boolean | Indicates whether the row grand total is included. |
| [isColumnGrandIncluded](#isColumnGrandIncluded--)| boolean | Indicates whether the column grand total is included. |
| [axisType](#axisType--)| PivotFieldType | Gets and sets the region of the PivotTable to which this rule applies. |
| [ruleType](#ruleType--)| PivotAreaType | Gets and sets the type of selection rule. |
| [isOutline](#isOutline--)| boolean | Indicates whether the rule refers to an area that is in outline mode. |

## Methods

| Method | Description |
| --- | --- |
| [select(PivotFieldType, number, PivotTableSelectionType)](#select-pivotfieldtype-number-pivottableselectiontype-)| Select the area with filters. |
| [selectField(PivotFieldType, string)](#selectField-pivotfieldtype-string-)| Select a field in the region as an area. |
| [selectField(PivotFieldType, PivotField)](#selectField-pivotfieldtype-pivotfield-)| Select a field in the region as an area. |
| [getCellAreas()](#getCellAreas--)| Gets cell areas of this pivot area. |


### constructor(PivotTable) {#constructor-pivottable-}

Presents the selected area of the PivotTable.

```javascript
constructor(table: PivotTable);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| table | [PivotTable](../pivottable/) |  |

### filters {#filters--}

Readonly. Gets all filters for this PivotArea.

```javascript
filters : PivotAreaFilterCollection;
```


### onlyData {#onlyData--}

Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels.

```javascript
onlyData : boolean;
```


### onlyLabel {#onlyLabel--}

Indicates whether only the data labels for an item selection are selected.

```javascript
onlyLabel : boolean;
```


### isRowGrandIncluded {#isRowGrandIncluded--}

Indicates whether the row grand total is included.

```javascript
isRowGrandIncluded : boolean;
```


### isColumnGrandIncluded {#isColumnGrandIncluded--}

Indicates whether the column grand total is included.

```javascript
isColumnGrandIncluded : boolean;
```


### axisType {#axisType--}

Gets and sets the region of the PivotTable to which this rule applies.

```javascript
axisType : PivotFieldType;
```


### ruleType {#ruleType--}

Gets and sets the type of selection rule.

```javascript
ruleType : PivotAreaType;
```


### isOutline {#isOutline--}

Indicates whether the rule refers to an area that is in outline mode.

```javascript
isOutline : boolean;
```


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

### selectField(PivotFieldType, string) {#selectField-pivotfieldtype-string-}

Select a field in the region as an area.

```javascript
selectField(axisType: PivotFieldType, fieldName: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | [PivotFieldType](../pivotfieldtype/) | The region type. |
| fieldName | string | The name of pivot field. |

### selectField(PivotFieldType, PivotField) {#selectField-pivotfieldtype-pivotfield-}

Select a field in the region as an area.

```javascript
selectField(axisType: PivotFieldType, field: PivotField) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | [PivotFieldType](../pivotfieldtype/) | The region type. |
| field | [PivotField](../pivotfield/) | The pivot field. |

### getCellAreas() {#getCellAreas--}

Gets cell areas of this pivot area.

```javascript
getCellAreas() : CellArea[];
```


**Returns**

[CellArea](../cellarea/)[]


