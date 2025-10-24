##Aspose::Cells::LoadFilter class
'Aspose::Cells::LoadFilter class. Represents the filter that provides options for loading data when loading workbook from template in C++.'
## LoadFilter class
Represents the filter that provides options for loading data when loading workbook from template.
```cpp
class LoadFilter
```
## Methods
| Method | Description |
| --- | --- |
| [GetLoadDataFilterOptions()](./getloaddatafilteroptions/) | Gets the filter options to denote what data should be loaded. |
| virtual [GetSheetsInLoadingOrder()](./getsheetsinloadingorder/) | Specifies the sheets(indices) and order to be loaded. Default is null, that denotes to load all sheets in the default order in template file. If not null and some sheet's index is not in the returned array, then the sheet will not be loaded. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [LoadFilter()](./loadfilter/) | Constructs one [LoadFilter](./) with default filter options [LoadDataFilterOptions::All](../loaddatafilteroptions/). |
| explicit [LoadFilter(LoadDataFilterOptions opts)](./loadfilter/) | Constructs one [LoadFilter](./) with given filter options. |
| [LoadFilter(const LoadFilter\& src)](./loadfilter/) |  |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const LoadFilter\& src)](./operator_asm/) |  |
| [SetLoadDataFilterOptions(LoadDataFilterOptions value)](./setloaddatafilteroptions/) | Sets the filter options to denote what data should be loaded. |
| virtual [StartSheet(Worksheet\& sheet)](./startsheet/) | Prepares filter options before loading given worksheet. User's implementation of [LoadFilter](./) can change the LoadDataFilterOptions here to denote how to load data for this worksheet. |
| [~LoadFilter()](./~loadfilter/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
| [_loadDataFilterOptions](./_loaddatafilteroptions/) | The default filter options used by this filter. |
## Remarks
User may specify the filter options or implement their own [LoadFilter](./) to specify how to load data.
## Examples
```cpp
Aspose::Cells::Startup();
//Custom LoadFilter implementation
class LoadFilterSheet : public LoadFilter
{
public:
void StartSheet(Worksheet& sheet)
{
if (sheet.GetName() == u"Sheet1")
{
SetLoadDataFilterOptions(LoadDataFilterOptions::All);
}
else
{
SetLoadDataFilterOptions(LoadDataFilterOptions::Structure);
}
}
};
//The following example shows how to determine the filter options according to worksheet's properties.
LoadOptions opts;
LoadFilterSheet filter;
opts.SetLoadFilter(&filter);
Workbook wb(u"template.xlsx", opts);
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
