---
title: LoadFilter class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 1010
url: /python-net/aspose.cells/loadfilter/
is_root: false
---

## LoadFilter class

Represents the filter that provides options for loading data when loading workbook from template.



The LoadFilter type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [LoadFilter()](/cells/python-net/aspose.cells/loadfilter/__init__/#) | Constructs one LoadFilter with default filter options LoadDataFilterOptions.All. |
| [LoadFilter(opts)](/cells/python-net/aspose.cells/loadfilter/__init__/#LoadDataFilterOptions) | Constructs one LoadFilter with given filter options. |


### Properties
| Property | Description |
| :- | :- |
| [load_data_filter_options](/cells/python-net/aspose.cells/loadfilter/load_data_filter_options) | The filter options to denote what data should be loaded. |
| [sheets_in_loading_order](/cells/python-net/aspose.cells/loadfilter/sheets_in_loading_order) | Specifies the sheets(indices) and order to be loaded.<br/>Default is null, that denotes to load all sheets in the default order in template file.<br/>If not null and some sheet's index is not in the returned array, then the sheet will not be loaded. |


### Methods
| Method | Description |
| :- | :- |
| [start_sheet(sheet)](/cells/python-net/aspose.cells/loadfilter/start_sheet/#Worksheet) | Prepares filter options before loading given worksheet.<br/>User's implementation of LoadFilter can change the LoadDataFilterOptions here<br/>to denote how to load data for this worksheet. |



### Remarks 


User may specify the filter options or implement their own LoadFilter to specify how to load data.

### See Also
* module [aspose.cells](..)
