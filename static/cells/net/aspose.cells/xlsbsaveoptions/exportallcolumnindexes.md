##XlsbSaveOptions.ExportAllColumnIndexes
XlsbSaveOptions property. Indicates whether exporting all column indexes for cells
## XlsbSaveOptions.ExportAllColumnIndexes property
Indicates whether exporting all column indexes for cells.
```csharp
public bool ExportAllColumnIndexes { get; set; }
```
### Remarks
The default value is true.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XlsbSaveOptionsPropertyExportAllColumnIndexesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some data
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue(2);
worksheet.Cells["C2"].PutValue(3);
XlsbSaveOptions saveOptions = new XlsbSaveOptions
{
ExportAllColumnIndexes = true // Demonstrate the property usage
};
workbook.Save("XlsbExportAllColumnIndexes.xlsb", saveOptions);
}
}
}
```
### See Also
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
