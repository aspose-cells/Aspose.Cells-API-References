##LoadOptions.AutoFilter
LoadOptions property. Indicates whether auto filtering the data when loading the files
## LoadOptions.AutoFilter property
Indicates whether auto filtering the data when loading the files.
```csharp
public bool AutoFilter { get; set; }
```
### Remarks
Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyAutoFilterDemo
{
public static void Run()
{
// Create load options and enable AutoFilter
LoadOptions options = new LoadOptions();
options.AutoFilter = true;
// Load workbook with AutoFilter enabled
Workbook workbook = new Workbook("example.xlsx", options);
// Access first worksheet and apply AutoFilter
Worksheet worksheet = workbook.Worksheets[0];
worksheet.AutoFilter.Range = "A1:D10";
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
