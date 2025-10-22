##XlsSaveOptions.WpsCompatibility
XlsSaveOptions property. Indicates whether to make the xls more compatible with WPS
## XlsSaveOptions.WpsCompatibility property
Indicates whether to make the xls more compatible with WPS.
```csharp
public bool WpsCompatibility { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XlsSaveOptionsPropertyWpsCompatibilityDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Test WPS Compatibility");
worksheet.Cells["B1"].PutValue(123.45);
// Set save options with WPS compatibility
XlsSaveOptions saveOptions = new XlsSaveOptions();
saveOptions.WpsCompatibility = true;
// Save the workbook
workbook.Save("output_with_wps_compatibility.xls", saveOptions);
Console.WriteLine("File saved with WPS compatibility enabled.");
}
}
}
```
### See Also
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
