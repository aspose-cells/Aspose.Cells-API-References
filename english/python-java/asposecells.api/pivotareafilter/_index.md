---
title: "PivotAreaFilter Class"
linktitle: "PivotAreaFilter"
articleTitle: "PivotAreaFilter"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the filter of PivotArea for PivotTable ."
type: docs
weight: 4450
url: /python-java/asposecells.api/pivotareafilter/
---

## PivotAreaFilter class

Represents the filter of PivotArea for PivotTable .

## Constructors

| Name | Description |
| --- | --- |
| [PivotAreaFilter](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [FieldIndex](#fieldindex) | int |  |
| [Selected](#selected) | boolean | Indicates whether this field has selection. Only works when the PivotTable is in Outline view. |

## Methods

| Name | Description |
| --- | --- |
| [isSubtotalSet](#issubtotalset) | Gets which subtotal is set for this filter. |
| [setSubtotals](#setsubtotals) | Subtotal for the filter. |

### PivotAreaFilter() {#constructor}

### PivotAreaFilter.FieldIndex property {#fieldindex}

**Type:** int

### PivotAreaFilter.Selected property {#selected}

Indicates whether this field has selection. Only works when the PivotTable is in Outline view.

**Type:** boolean

### isSubtotalSet(subtotalType) {#issubtotalset}

Gets which subtotal is set for this filter.

| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | int | A PivotFieldSubtotalType value. The subtotal function type. |

### setSubtotals(subtotalType, shown) {#setsubtotals}

Subtotal for the filter.

| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | int | A PivotFieldSubtotalType value. The subtotal function. |
| shown | boolean | Indicates if showing this subtotal data. |
