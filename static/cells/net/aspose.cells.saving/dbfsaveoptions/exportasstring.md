##DbfSaveOptions.ExportAsString
DbfSaveOptions property. Indicates whether exporting as string value
## DbfSaveOptions.ExportAsString property
Indicates whether exporting as string value
```csharp
public bool ExportAsString { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Saving;
using System;
public class DbfSaveOptionsPropertyExportAsStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with mixed types
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue(123.45);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("TextValue");
// Create DbfSaveOptions instance
DbfSaveOptions options = new DbfSaveOptions();
// Display current ExportAsString value
Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);
// Set ExportAsString to true (all values will be exported as strings)
options.ExportAsString = true;
Console.WriteLine("ExportAsString set to: " + options.ExportAsString);
// Save with ExportAsString = true
workbook.Save("ExportAsStringTrue.dbf", options);
// Set ExportAsString to false (values will maintain their original types)
options.ExportAsString = false;
Console.WriteLine("ExportAsString set to: " + options.ExportAsString);
// Save with ExportAsString = false
workbook.Save("ExportAsStringFalse.dbf", options);
}
}
}
```
### See Also
* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
