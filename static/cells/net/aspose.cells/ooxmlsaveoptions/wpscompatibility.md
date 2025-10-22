##OoxmlSaveOptions.WpsCompatibility
OoxmlSaveOptions property. Indicates whether to make the xls more compatible with WPS
## OoxmlSaveOptions.WpsCompatibility property
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
public class OoxmlSaveOptionsPropertyWpsCompatibilityDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet and add sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test WPS Compatibility");
// Create OOXML save options and enable WPS compatibility
OoxmlSaveOptions options = new OoxmlSaveOptions();
options.WpsCompatibility = true;
// Save the workbook with WPS compatibility
workbook.Save("output_with_wps_compatibility.xlsx", options);
Console.WriteLine("Workbook saved with WPS compatibility enabled.");
}
}
}
```
### See Also
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
