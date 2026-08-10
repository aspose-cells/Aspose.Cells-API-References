---
title: "LoadFilter Class"
linktitle: "LoadFilter"
articleTitle: "LoadFilter"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the filter that provides options for loading data when loading workbook from template."
type: docs
weight: 3470
url: /php/aspose.cells/loadfilter/
---

## LoadFilter class

Represents the filter that provides options for loading data when loading workbook from template.

## Constructors

| Name | Description |
| --- | --- |
| [LoadFilter](#constructor) | Constructs one LoadFilter with default filter options LoadDataFilterOptions.All. |
| [LoadFilter](#constructor) | Constructs one LoadFilter with given filter options. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [LoadDataFilterOptions](#loaddatafilteroptions) | Number | The filter options to denote what data should be loaded. The value of the property is LoadDataFilterOptions integer cons |
| [SheetsInLoadingOrder](#sheetsinloadingorder) | int[] | Specifies the sheets(indices) and order to be loaded. Default is null, that denotes to load all sheets in the default or |

## Methods

| Name | Description |
| --- | --- |
| [startSheet](#startsheet) | Prepares filter options before loading given worksheet. User's implementation of LoadFilter can change the LoadDataFilte |

### LoadFilter() (1 of 2) {#constructor}

Constructs one LoadFilter with default filter options LoadDataFilterOptions.All.

---

### LoadFilter(opts) (2 of 2) {#constructor-1}

Constructs one LoadFilter with given filter options.

| Parameter | Type | Description |
| --- | --- | --- |
| opts | Number | A LoadDataFilterOptions value. the default filter options |

### LoadFilter.LoadDataFilterOptions property {#loaddatafilteroptions}

The filter options to denote what data should be loaded. The value of the property is LoadDataFilterOptions integer constant.

**Type:** Number

### LoadFilter.SheetsInLoadingOrder property {#sheetsinloadingorder}

Specifies the sheets(indices) and order to be loaded. Default is null, that denotes to load all sheets in the default order in template file. If not null and some sheet's index is not in the returned array, then the sheet will not be loaded.

**Type:** int[]

### startSheet(sheet) {#startsheet}

Prepares filter options before loading given worksheet. User's implementation of LoadFilter can change the LoadDataFilterOptions here to denote how to load data for this worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| sheet | Worksheet | The worksheet to be loaded. There are only few properties can be used for the given worksheet object here because most data and properties have not been loaded. The available properties are: Name, Index, VisibilityType |
