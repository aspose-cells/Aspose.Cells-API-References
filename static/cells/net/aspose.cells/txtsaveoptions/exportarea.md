##TxtSaveOptions.ExportArea
TxtSaveOptions property. The range of cells to be exported
## TxtSaveOptions.ExportArea property
The range of cells to be exported.
```csharp
public CellArea ExportArea { get; set; }
```
### Remarks
If the exported area has been specified, [`TrimLeadingBlankRowAndColumn`](../trimleadingblankrowandcolumn/) will takes no effect.
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtSaveOptionsPropertyExportAreaDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate cells with data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Laptop");
worksheet.Cells["B2"].PutValue(999.99);
worksheet.Cells["A3"].PutValue("Phone");
worksheet.Cells["B3"].PutValue(699.99);
worksheet.Cells["A4"].PutValue("Tablet");
worksheet.Cells["B4"].PutValue(399.99);
// Configure text save options with ExportArea
TxtSaveOptions saveOptions = new TxtSaveOptions
{
Separator = '\t',
ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
};
// Save only the specified area (first 3 rows, first 2 columns)
workbook.Save("ExportedData.txt", saveOptions);
Console.WriteLine("Data exported successfully with ExportArea restriction.");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
