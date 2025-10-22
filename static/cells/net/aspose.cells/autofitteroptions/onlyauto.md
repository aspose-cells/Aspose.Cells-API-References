##AutoFitterOptions.OnlyAuto
AutoFitterOptions property. Indicates whether only fit the rows which height are not customed
## AutoFitterOptions.OnlyAuto property
Indicates whether only fit the rows which height are not customed.
```csharp
public bool OnlyAuto { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFitterOptionsPropertyOnlyAutoDemo
{
public static void Run()
{
// Create load options and set OnlyAuto property
LoadOptions loadOptions = new LoadOptions();
loadOptions.AutoFitterOptions = new AutoFitterOptions();
loadOptions.AutoFitterOptions.OnlyAuto = true;
// Load workbook with auto-fit options
Workbook workbook = new Workbook("example.xml", loadOptions);
// Demonstrate auto-fitting by checking column width
Console.WriteLine("Column width after auto-fit: " +
workbook.Worksheets[0].Cells.GetColumnWidthPixel(0));
// Save and reload to verify persistence
workbook.Save("example_output.xlsx");
Workbook reloaded = new Workbook("example_output.xlsx");
Console.WriteLine("Reloaded column width: " +
reloaded.Worksheets[0].Cells.GetColumnWidthPixel(0));
}
}
}
```
### See Also
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
