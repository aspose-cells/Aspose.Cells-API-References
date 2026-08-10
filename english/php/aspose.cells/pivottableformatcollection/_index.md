---
title: "PivotTableFormatCollection Class"
linktitle: "PivotTableFormatCollection"
articleTitle: "PivotTableFormatCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the collection of formats applied to PivotTable."
type: docs
weight: 4870
url: /php/aspose.cells/pivottableformatcollection/
---

## PivotTableFormatCollection class

Represents the collection of formats applied to PivotTable.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | Number |  |
| [Item (int)](#itemint) | PivotTableFormat | Gets the format by the index. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Add a PivotTableFormat . |
| [formatArea](#formatarea) | Formats selected area. |
| [clear](#clear) |  |
| [removeAt](#removeat) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### PivotTableFormatCollection.Count property {#count}

**Type:** Number

### PivotTableFormatCollection.Item (int) property {#itemint}

Gets the format by the index.

**Type:** PivotTableFormat

### add() (1 of 2) {#add}

Add a PivotTableFormat .

**Returns:** The index of new format.

---

### add(value) (2 of 2) {#add-1}

Reserved for internal use.

### formatArea(axisType, fieldPosition, subtotalType, selectionType, isGrandRow, isGrandColumn, style) {#formatarea}

Formats selected area.

| Parameter | Type | Description |
| --- | --- | --- |
| axisType | Number | A PivotFieldType value. The region of the PivotTable to which this rule applies. |
| fieldPosition | Number | Position of the field within the axis to which this rule applies. |
| subtotalType | Number | A PivotFieldSubtotalType value. The subtotal filter type of the pivot field |
| selectionType | Number | A PivotTableSelectionType value. Indicates how to select data. |
| isGrandRow | boolean | Indicates whether selecting grand total rows. |
| isGrandColumn | boolean | Indicates whether selecting grand total columns. |
| style | Style | The style which appies to the area of the pivot table. |

### clear() {#clear}

### removeAt(index) {#removeat}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
