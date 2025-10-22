##OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink
OdsLoadOptions property. Indicates whether applying the default style of the Excel to hyperlink
## OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink property
Indicates whether applying the default style of the Excel to hyperlink.
```csharp
public bool ApplyExcelDefaultStyleToHyperlink { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OdsLoadOptionsPropertyApplyExcelDefaultStyleToHyperlinkDemo
{
public static void Run()
{
// Create an instance of OdsLoadOptions
OdsLoadOptions loadOptions = new OdsLoadOptions();
// Set ApplyExcelDefaultStyleToHyperlink property
loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
// Load an ODS file with the specified options
Workbook workbook = new Workbook("sample.ods", loadOptions);
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a hyperlink to demonstrate the style application
worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
// Save the workbook to a new file
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
