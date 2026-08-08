---
title: "LoadFilter"
linktitle: "LoadFilter"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the filter that provides options for loading data when loading workbook from template."
type: docs
weight: 2140
url: /nodejs/aspose.cells/loadfilter/
---

## LoadFilter class

Represents the filter that provides options for loading data when loading workbook from template. User may specify the filter options or implement their own LoadFilter to specify how to load data.

```js
new LoadFilter()
```

Constructs one LoadFilter with default filter options LoadDataFilterOptions.All.

## Methods

| Name | Description |
| --- | --- |
| [constructor_overload$1(opts)](./constructor-overload1/) | Constructs one LoadFilter with given filter options. |
| [getLoadDataFilterOptions()](./getloaddatafilteroptions/) | The filter options to denote what data should be loaded. The value of the property is LoadDataFilterOptions integer cons |
| [getSheetsInLoadingOrder()](./getsheetsinloadingorder/) | Specifies the sheets(indices) and order to be loaded. Default is null, that denotes to load all sheets in the default or |
| [setLoadDataFilterOptions()](./setloaddatafilteroptions/) | The filter options to denote what data should be loaded. The value of the property is LoadDataFilterOptions integer cons |
| [startSheet(sheet)](./startsheet/) | Prepares filter options before loading given worksheet. User's implementation of LoadFilter can change the LoadDataFilte |
