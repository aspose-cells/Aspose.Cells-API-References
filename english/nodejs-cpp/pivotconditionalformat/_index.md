---
title: PivotConditionalFormat
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a PivotTable Format Condition in PivotFormatCondition Collection.
type: docs
url: /nodejs-cpp/pivotconditionalformat/
---

## PivotConditionalFormat class

Represents a PivotTable Format Condition in PivotFormatCondition Collection.

```javascript
class PivotConditionalFormat;
```


## Methods

| Method | Description |
| --- | --- |
| [getPivotAreas()](#getPivotAreas--)| Gets all pivot areas. |
| [getFormatConditions()](#getFormatConditions--)| Get conditions for the pivot table conditional format . |
| [getScopeType()](#getScopeType--)| Get and set scope type for the pivot table conditional format . |
| [setScopeType(PivotConditionFormatScopeType)](#setScopeType-pivotconditionformatscopetype-)| Get and set scope type for the pivot table conditional format . |
| [getRuleType()](#getRuleType--)| Get and set rule type for the pivot table condition format . |
| [setRuleType(PivotConditionFormatRuleType)](#setRuleType-pivotconditionformatruletype-)| Get and set rule type for the pivot table condition format . |
| [getCellAreas()](#getCellAreas--)| Gets all cell areas where this conditional format applies to. |
| [addCellArea(CellArea)](#addCellArea-cellarea-)| Adds an area based on pivot table view. |
| [addFieldArea(PivotFieldType, string)](#addFieldArea-pivotfieldtype-string-)| Adds an area of pivot field. |
| [addFieldArea(PivotFieldType, PivotField)](#addFieldArea-pivotfieldtype-pivotfield-)| Adds an area of pivot field. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getPivotAreas() {#getPivotAreas--}

Gets all pivot areas.

```javascript
getPivotAreas() : PivotAreaCollection;
```


**Returns**

[PivotAreaCollection](../pivotareacollection/)

### getFormatConditions() {#getFormatConditions--}

Get conditions for the pivot table conditional format .

```javascript
getFormatConditions() : FormatConditionCollection;
```


**Returns**

[FormatConditionCollection](../formatconditioncollection/)

### getScopeType() {#getScopeType--}

Get and set scope type for the pivot table conditional format .

```javascript
getScopeType() : PivotConditionFormatScopeType;
```


**Returns**

[PivotConditionFormatScopeType](../pivotconditionformatscopetype/)

### setScopeType(PivotConditionFormatScopeType) {#setScopeType-pivotconditionformatscopetype-}

Get and set scope type for the pivot table conditional format .

```javascript
setScopeType(value: PivotConditionFormatScopeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotConditionFormatScopeType](../pivotconditionformatscopetype/) | The value to set. |

### getRuleType() {#getRuleType--}

Get and set rule type for the pivot table condition format .

```javascript
getRuleType() : PivotConditionFormatRuleType;
```


**Returns**

[PivotConditionFormatRuleType](../pivotconditionformatruletype/)

### setRuleType(PivotConditionFormatRuleType) {#setRuleType-pivotconditionformatruletype-}

Get and set rule type for the pivot table condition format .

```javascript
setRuleType(value: PivotConditionFormatRuleType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotConditionFormatRuleType](../pivotconditionformatruletype/) | The value to set. |

### getCellAreas() {#getCellAreas--}

Gets all cell areas where this conditional format applies to.

```javascript
getCellAreas() : CellArea[];
```


**Returns**

[CellArea](../cellarea/)[]

### addCellArea(CellArea) {#addCellArea-cellarea-}

Adds an area based on pivot table view.

```javascript
addCellArea(ca: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../cellarea/) | The cell area. |

### addFieldArea(PivotFieldType, string) {#addFieldArea-pivotfieldtype-string-}

Adds an area of pivot field.

```javascript
addFieldArea(axisType: PivotFieldType, fieldName: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | [PivotFieldType](../pivotfieldtype/) | The region type. |
| fieldName | string | The name of pivot field. |

### addFieldArea(PivotFieldType, PivotField) {#addFieldArea-pivotfieldtype-pivotfield-}

Adds an area of pivot field.

```javascript
addFieldArea(axisType: PivotFieldType, field: PivotField) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | [PivotFieldType](../pivotfieldtype/) | The region type. |
| field | [PivotField](../pivotfield/) | The pivot field. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



