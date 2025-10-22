##HtmlSaveOptions.ExportWorksheetProperties
HtmlSaveOptions property. Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel please keep the default value
## HtmlSaveOptions.ExportWorksheetProperties property
Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.
```csharp
public bool ExportWorksheetProperties { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportWorksheetPropertiesDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test Data");
// Set HTML save options with ExportWorksheetProperties disabled
HtmlSaveOptions options = new HtmlSaveOptions();
options.ExportWorksheetProperties = false;
// Save with worksheet properties disabled
workbook.Save("output_without_worksheet_props.html", options);
// Enable worksheet properties export
options.ExportWorksheetProperties = true;
// Save with worksheet properties enabled
workbook.Save("output_with_worksheet_props.html", options);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
