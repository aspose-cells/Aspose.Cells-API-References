##Class LoadFilter
Aspose.Cells.LoadFilter class. Represents the filter that provides options for loading data when loading workbook from template
## LoadFilter class
Represents the filter that provides options for loading data when loading workbook from template.
```csharp
public class LoadFilter
```
## Constructors
| Name | Description |
| --- | --- |
| [LoadFilter](loadfilter/#constructor)() | Constructs one LoadFilter with default filter options LoadDataFilterOptions.All. |
| [LoadFilter](loadfilter/#constructor_1)(LoadDataFilterOptions) | Constructs one LoadFilter with given filter options. |
## Properties
| Name | Description |
| --- | --- |
| [LoadDataFilterOptions](../../aspose.cells/loadfilter/loaddatafilteroptions/) { get; set; } | The filter options to denote what data should be loaded. |
| virtual [SheetsInLoadingOrder](../../aspose.cells/loadfilter/sheetsinloadingorder/) { get; } | Specifies the sheets(indices) and order to be loaded. Default is null, that denotes to load all sheets in the default order in template file. If not null and some sheet's index is not in the returned array, then the sheet will not be loaded. |
## Methods
| Name | Description |
| --- | --- |
| virtual [StartSheet](../../aspose.cells/loadfilter/startsheet/)(Worksheet) | Prepares filter options before loading given worksheet. User's implementation of LoadFilter can change the LoadDataFilterOptions here to denote how to load data for this worksheet. |
### Remarks
User may specify the filter options or implement their own LoadFilter to specify how to load data.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LoadFilterDemo
{
public static void LoadFilterExample()
{
// Create LoadOptions and set LoadFilter
LoadOptions opts = new LoadOptions();
opts.LoadFilter = new CustomLoadFilter();
// Load the workbook with the specified LoadOptions
Workbook wb = new Workbook("LoadFilterExample_original.xlsx", opts);
// Save the workbook to see the effect of LoadFilter
wb.Save("LoadFilterExample.xlsx");
}
// Custom LoadFilter implementation
public class CustomLoadFilter : LoadFilter
{
public override void StartSheet(Worksheet sheet)
{
if (sheet.Name == "Sheet1")
{
LoadDataFilterOptions = LoadDataFilterOptions.All;
}
else
{
LoadDataFilterOptions = LoadDataFilterOptions.Structure;
}
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
