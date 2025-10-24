##Workbook.IsLicensed
Workbook property. Indicates whether license is set
## Workbook.IsLicensed property
Indicates whether license is set.
```csharp
public bool IsLicensed { get; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyIsLicensedDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Set some basic properties to demonstrate the workbook is being used
wb.Worksheets[0].Name = "Sheet1";
wb.Worksheets[0].Cells[0, 0].PutValue("Sample Data");
// Check if the workbook is licensed
Console.WriteLine($"IsLicensed: {wb.IsLicensed}");
// Demonstrate different behavior based on license status
if (wb.IsLicensed)
{
Console.WriteLine("Running in licensed mode - full features available");
}
else
{
Console.WriteLine("Running in evaluation mode - watermarks will appear");
}
// Save to memory stream to demonstrate functionality
using (MemoryStream ms = new MemoryStream())
{
wb.Save(ms, SaveFormat.Xlsx);
Console.WriteLine($"Workbook saved successfully (Size: {ms.Length} bytes)");
}
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
