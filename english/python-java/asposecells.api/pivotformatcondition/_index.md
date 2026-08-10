---
title: "PivotFormatCondition Class"
linktitle: "PivotFormatCondition"
articleTitle: "PivotFormatCondition"
second_title: "Aspose.Cells for Python via Java"
description: "Represents a PivotTable Format Condition in PivotFormatCondition Collection."
type: docs
weight: 4670
url: /python-java/asposecells.api/pivotformatcondition/
---

## PivotFormatCondition class

Represents a PivotTable Format Condition in PivotFormatCondition Collection.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [ScopeType](#scopetype) | int | Get and set scope type for the pivot table condition format . The value of the property is PivotConditionFormatScopeType |
| [RuleType](#ruletype) | int | Get and set rule type for the pivot table condition format . The value of the property is PivotConditionFormatRuleType i |
| [FormatConditions](#formatconditions) | FormatConditionCollection | Get formatconditions for the pivot table condition format . |

## Methods

| Name | Description |
| --- | --- |
| [addDataAreaCondition](#adddataareacondition) | Adds PivotTable conditional format limit in the data fields. |
| [addRowAreaCondition](#addrowareacondition) | Adds PivotTable conditional format limit in the row fields. |
| [addColumnAreaCondition](#addcolumnareacondition) | Adds PivotTable conditional format limit in the column fields. |
| [setConditionalAreas](#setconditionalareas) | Sets conditional areas of PivotFormatCondition object. |

### PivotFormatCondition.ScopeType property {#scopetype}

Get and set scope type for the pivot table condition format . The value of the property is PivotConditionFormatScopeType integer constant.

**Type:** int

### PivotFormatCondition.RuleType property {#ruletype}

Get and set rule type for the pivot table condition format . The value of the property is PivotConditionFormatRuleType integer constant.

**Type:** int

### PivotFormatCondition.FormatConditions property {#formatconditions}

Get formatconditions for the pivot table condition format .

**Type:** FormatConditionCollection

### addDataAreaCondition(fieldName) (1 of 2) {#adddataareacondition}

Adds PivotTable conditional format limit in the data fields.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | String | The name of PivotField. |

---

### addDataAreaCondition(dataField) (2 of 2) {#adddataareacondition-1}

Adds PivotTable conditional format limit in the data fields.

| Parameter | Type | Description |
| --- | --- | --- |
| dataField | PivotField | The PivotField in the data fields. |

### addRowAreaCondition(fieldName) (1 of 2) {#addrowareacondition}

Adds PivotTable conditional format limit in the row fields.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | String | The name of PivotField. |

---

### addRowAreaCondition(rowField) (2 of 2) {#addrowareacondition-1}

Adds PivotTable conditional format limit in the row fields.

| Parameter | Type | Description |
| --- | --- | --- |
| rowField | PivotField | The PivotField in the row fields. |

### addColumnAreaCondition(fieldName) (1 of 2) {#addcolumnareacondition}

Adds PivotTable conditional format limit in the column fields.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | String | The name of PivotField. |

---

### addColumnAreaCondition(columnField) (2 of 2) {#addcolumnareacondition-1}

Adds PivotTable conditional format limit in the column fields.

| Parameter | Type | Description |
| --- | --- | --- |
| columnField | PivotField | The PivotField in the column fields. |

### setConditionalAreas() {#setconditionalareas}

Sets conditional areas of PivotFormatCondition object.
