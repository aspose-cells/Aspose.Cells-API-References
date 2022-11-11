---
title: LoadFilter
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 1010
url: /cells/python-net/aspose.cells/loadfilter/
---

## LoadFilter class

Represents the filter that provides options for loading data when loading workbook from template.

The LoadFilter type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|LoadFilter()|Constructs one LoadFilter with default filter options LoadDataFilterOptions.All.|
|LoadFilter(opts)|Initializes a new instance of the LoadFilter class|
## Properties
| Name | Description |
| :- | :- |
|load_data_filter_options|The filter options to denote what data should be loaded.|
|sheets_in_loading_order|Specifies the sheets(indices) and order to be loaded.<br/>            Default is null, that denotes to load all sheets in the default order in template file.<br/>            If not null and some sheet's index is not in the returned array, then the sheet will not be loaded.|
## Methods
| Name | Description |
| :- | :- |
|start_sheet(sheet)|Prepares filter options before loading given worksheet.<br/>            User's implementation of LoadFilter can change the LoadDataFilterOptions here<br/>            to denote how to load data for this worksheet.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

