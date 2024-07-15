---
title: PivotFormatCondition
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a PivotTable Format Condition in PivotFormatCondition Collection.
type: docs
url: /nodejs-cpp/pivotformatcondition/
---

## PivotFormatCondition class

Represents a PivotTable Format Condition in PivotFormatCondition Collection.

```javascript
class PivotFormatCondition;
```


## Methods

| Method | Description |
| --- | --- |
| [getScopeType()](#getScopeType--)| Get and set scope type for the pivot table condition format . |
| [setScopeType(PivotConditionFormatScopeType)](#setScopeType-pivotconditionformatscopetype-)| Get and set scope type for the pivot table condition format . |
| [getRuleType()](#getRuleType--)| Get and set rule type for the pivot table condition format . |
| [setRuleType(PivotConditionFormatRuleType)](#setRuleType-pivotconditionformatruletype-)| Get and set rule type for the pivot table condition format . |
| [getFormatConditions()](#getFormatConditions--)| Get formatconditions for the pivot table condition format . |
| [addDataAreaCondition(string)](#addDataAreaCondition-string-)| Adds PivotTable conditional format limit in the data fields. |
| [addDataAreaCondition(PivotField)](#addDataAreaCondition-pivotfield-)| Adds PivotTable conditional format limit in the data fields. |
| [addRowAreaCondition(string)](#addRowAreaCondition-string-)| Adds PivotTable conditional format limit in the row fields. |
| [addRowAreaCondition(PivotField)](#addRowAreaCondition-pivotfield-)| Adds PivotTable conditional format limit in the row fields. |
| [addColumnAreaCondition(string)](#addColumnAreaCondition-string-)| Adds PivotTable conditional format limit in the column fields. |
| [addColumnAreaCondition(PivotField)](#addColumnAreaCondition-pivotfield-)| Adds PivotTable conditional format limit in the column fields. |
| [setConditionalAreas()](#setConditionalAreas--)| Sets conditional areas of PivotFormatCondition object. |


### getScopeType() {#getScopeType--}

Get and set scope type for the pivot table condition format .

```javascript
getScopeType() : PivotConditionFormatScopeType;
```


**Returns**

[PivotConditionFormatScopeType](../pivotconditionformatscopetype/)

### setScopeType(PivotConditionFormatScopeType) {#setScopeType-pivotconditionformatscopetype-}

Get and set scope type for the pivot table condition format .

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

### getFormatConditions() {#getFormatConditions--}

Get formatconditions for the pivot table condition format .

```javascript
getFormatConditions() : FormatConditionCollection;
```


**Returns**

[FormatConditionCollection](../formatconditioncollection/)

### addDataAreaCondition(string) {#addDataAreaCondition-string-}

Adds PivotTable conditional format limit in the data fields.

```javascript
addDataAreaCondition(fieldName: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | string | The name of PivotField. |

### addDataAreaCondition(PivotField) {#addDataAreaCondition-pivotfield-}

Adds PivotTable conditional format limit in the data fields.

```javascript
addDataAreaCondition(dataField: PivotField) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dataField | [PivotField](../pivotfield/) | The PivotField in the data fields. |

### addRowAreaCondition(string) {#addRowAreaCondition-string-}

Adds PivotTable conditional format limit in the row fields.

```javascript
addRowAreaCondition(fieldName: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | string | The name of PivotField. |

### addRowAreaCondition(PivotField) {#addRowAreaCondition-pivotfield-}

Adds PivotTable conditional format limit in the row fields.

```javascript
addRowAreaCondition(rowField: PivotField) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowField | [PivotField](../pivotfield/) | The PivotField in the row fields. |

### addColumnAreaCondition(string) {#addColumnAreaCondition-string-}

Adds PivotTable conditional format limit in the column fields.

```javascript
addColumnAreaCondition(fieldName: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | string | The name of PivotField. |

### addColumnAreaCondition(PivotField) {#addColumnAreaCondition-pivotfield-}

Adds PivotTable conditional format limit in the column fields.

```javascript
addColumnAreaCondition(columnField: PivotField) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnField | [PivotField](../pivotfield/) | The PivotField in the column fields. |

### setConditionalAreas() {#setConditionalAreas--}

Sets conditional areas of PivotFormatCondition object.

```javascript
setConditionalAreas() : void;
```



