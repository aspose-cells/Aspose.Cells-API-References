##LoadFilter.LoadFilter
LoadFilter constructor. Constructs one LoadFilter with default filter options LoadDataFilterOptions.All
## LoadFilter() {#constructor}
Constructs one LoadFilter with default filter options LoadDataFilterOptions.All.
```csharp
public LoadFilter()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadFilterMethodCtorDemo
{
public static void Run()
{
// Create a new LoadFilter with default constructor
LoadFilter filter = new LoadFilter();
// Create load options and assign the filter
LoadOptions loadOptions = new LoadOptions();
loadOptions.LoadFilter = filter;
// Load workbook with the filter
Workbook workbook = new Workbook("sample.xlsx", loadOptions);
// Demonstrate usage by counting worksheets
Console.WriteLine("Number of worksheets loaded: " + workbook.Worksheets.Count);
// Show filtered cell data (all cells loaded by default)
foreach (Worksheet sheet in workbook.Worksheets)
{
Console.WriteLine($"Worksheet '{sheet.Name}' has {sheet.Cells.Count} cells");
}
}
}
}
```
### See Also
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## LoadFilter(LoadDataFilterOptions) {#constructor_1}
Constructs one LoadFilter with given filter options.
```csharp
public LoadFilter(LoadDataFilterOptions opts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| opts | LoadDataFilterOptions | the default filter options |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LoadFilterMethodCtorWithLoadDataFilterOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare data for the method parameters (LoadDataFilterOptions)
LoadDataFilterOptions filterOptions = LoadDataFilterOptions.CellData | LoadDataFilterOptions.Chart;
try
{
// Call the #ctor method with the specific parameter types
LoadFilter loadFilter = new LoadFilter(filterOptions);
// Process or display the result
Console.WriteLine("LoadFilter created successfully with LoadDataFilterOptions: " + filterOptions);
// Show the effect of the method call
Console.WriteLine("LoadDataFilterOptions set to: " + loadFilter.LoadDataFilterOptions);
}
catch (Exception ex)
{
Console.WriteLine($"Error creating LoadFilter: {ex.Message}");
}
// Save the result
workbook.Save("LoadFilterCtorWithLoadDataFilterOptionsDemo.xlsx");
}
}
}
```
### See Also
* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
