##LoadOptions.CultureInfo
LoadOptions property. Gets or sets the regional settings used for the Workbook that will be loaded
## LoadOptions.CultureInfo property
Gets or sets the regional settings used for the Workbook that will be loaded.
```csharp
public CultureInfo CultureInfo { get; set; }
```
### Remarks
This property has the same effect with [`Region`](../region/) for setting regional settings.
### Examples
```csharp
using System;
using System.Globalization;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyCultureInfoDemo
{
public static void Run()
{
// Create sample Excel file
Workbook sampleWorkbook = new Workbook();
sampleWorkbook.Worksheets[0].Cells["A1"].PutValue(1234.56);
sampleWorkbook.Save("sample.xlsx", SaveFormat.Xlsx);
// Load with specific culture
LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
options.CultureInfo = new CultureInfo("de-DE"); // German culture uses comma as decimal separator
Workbook workbook = new Workbook("sample.xlsx", options);
Console.WriteLine("Value with German culture: " + workbook.Worksheets[0].Cells["A1"].StringValue);
}
}
}
```
### See Also
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
