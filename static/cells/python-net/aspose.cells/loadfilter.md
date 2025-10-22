##LoadFilter class
## LoadFilter class
Represents the filter that provides options for loading data when loading workbook from template.
The LoadFilter type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/loadfilter/__init__/#) | Constructs one LoadFilter with default filter options LoadDataFilterOptions.All. |
| [`__init__(self, opts)`](/cells/python-net/aspose.cells/loadfilter/__init__/#aspose.cells.loaddatafilteroptions) | Constructs one LoadFilter with given filter options. |
### Properties
| Property | Description |
| :- | :- |
| [load_data_filter_options](/cells/python-net/aspose.cells/loadfilter/load_data_filter_options) | The filter options to denote what data should be loaded. |
| [sheets_in_loading_order](/cells/python-net/aspose.cells/loadfilter/sheets_in_loading_order) | Specifies the sheets(indices) and order to be loaded.
### Methods
| Method | Description |
| :- | :- |
| [`start_sheet(self, sheet)`](/cells/python-net/aspose.cells/loadfilter/start_sheet/#aspose.cells.worksheet) | Prepares filter options before loading given worksheet.
### Remarks
User may specify the filter options or implement their own LoadFilter to specify how to load data.
### See Also
* module [`aspose.cells`](..)
