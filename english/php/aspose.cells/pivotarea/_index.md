---
title: "PivotArea Class"
linktitle: "PivotArea"
articleTitle: "PivotArea"
second_title: "Aspose.Cells for PHP via Java"
description: "Presents the selected area of the PivotTable."
type: docs
weight: 4430
url: /php/aspose.cells/pivotarea/
---

## PivotArea class

Presents the selected area of the PivotTable.

## Constructors

| Name | Description |
| --- | --- |
| [PivotArea](#constructor) | Presents the selected area of the PivotTable. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Filters](#filters) | PivotAreaFilterCollection | Gets all filters for this PivotArea. |
| [OnlyData](#onlydata) | boolean | Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not in |
| [OnlyLabel](#onlylabel) | boolean | Indicates whether only the data labels for an item selection are selected. |
| [IsRowGrandIncluded](#isrowgrandincluded) | boolean | Indicates whether the row grand total is included. |
| [IsColumnGrandIncluded](#iscolumngrandincluded) | boolean | Indicates whether the column grand total is included. |
| [AxisType](#axistype) | Number | Gets and sets the region of the PivotTable to which this rule applies. The value of the property is PivotFieldType integ |
| [RuleType](#ruletype) | Number | Gets and sets the type of selection rule. The value of the property is PivotAreaType integer constant. |
| [IsOutline](#isoutline) | boolean | Indicates whether the rule refers to an area that is in outline mode. |

## Methods

| Name | Description |
| --- | --- |
| [select](#select) | Select the area with filters. |
| [selectField](#selectfield) |  |
| [getCellAreas](#getcellareas) |  |

### PivotArea(table) {#constructor}

Presents the selected area of the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| table | PivotTable |  |

### PivotArea.Filters property {#filters}

Gets all filters for this PivotArea.

**Type:** PivotAreaFilterCollection

### PivotArea.OnlyData property {#onlydata}

Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels.

**Type:** boolean

### PivotArea.OnlyLabel property {#onlylabel}

Indicates whether only the data labels for an item selection are selected.

**Type:** boolean

### PivotArea.IsRowGrandIncluded property {#isrowgrandincluded}

Indicates whether the row grand total is included.

**Type:** boolean

### PivotArea.IsColumnGrandIncluded property {#iscolumngrandincluded}

Indicates whether the column grand total is included.

**Type:** boolean

### PivotArea.AxisType property {#axistype}

Gets and sets the region of the PivotTable to which this rule applies. The value of the property is PivotFieldType integer constant.

**Type:** Number

### PivotArea.RuleType property {#ruletype}

Gets and sets the type of selection rule. The value of the property is PivotAreaType integer constant.

**Type:** Number

### PivotArea.IsOutline property {#isoutline}

Indicates whether the rule refers to an area that is in outline mode.

**Type:** boolean

### select(axisType, fieldPosition, selectionType) {#select}

Select the area with filters.

| Parameter | Type | Description |
| --- | --- | --- |
| axisType | Number | A PivotFieldType value. The region of the PivotTable to which this rule applies. |
| fieldPosition | Number | Position of the field within the axis to which this rule applies. |
| selectionType | Number | A PivotTableSelectionType value. Specifies what can be selected in a PivotTable during a structured selection. |

### selectField(axisType, fieldName) (1 of 2) {#selectfield}

---

### selectField(axisType, field) (2 of 2) {#selectfield-1}

### getCellAreas() {#getcellareas}
