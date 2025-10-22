##LoadOptions.AutoFitterOptions
LoadOptions property. Gets and sets the auto fitter options
## LoadOptions.AutoFitterOptions property
Gets and sets the auto fitter options
```csharp
public AutoFitterOptions AutoFitterOptions { get; set; }
```
### Remarks
Only for xlsx ,spreadsheetML file now.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyAutoFitterOptionsDemo
{
public static void Run()
{
// Create AutoFitterOptions and set properties
AutoFitterOptions options = new AutoFitterOptions();
options.AutoFitMergedCells = true;
options.OnlyAuto = false;
// Create LoadOptions and assign AutoFitterOptions
LoadOptions loadOptions = new LoadOptions();
loadOptions.AutoFitterOptions = options;
// Load workbook with the specified options
Workbook workbook = new Workbook("example.xlsx", loadOptions);
// Demonstrate auto-fitting by getting row height
double rowHeight = workbook.Worksheets[0].Cells.GetRowHeight(0);
Console.WriteLine("Row height after auto-fitting: " + rowHeight);
}
}
}
```
### See Also
* class [AutoFitterOptions](../../autofitteroptions/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
