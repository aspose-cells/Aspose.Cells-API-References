##Worksheet.Workbook
Worksheet property. Gets the workbook object which contains this sheet
## Worksheet.Workbook property
Gets the workbook object which contains this sheet.
```csharp
public Workbook Workbook { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyWorkbookDemo
{
public static void Run()
{
// Create a source workbook and get a worksheet
Workbook sourceWorkbook = new Workbook();
Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
// Add sample data to source worksheet
sourceSheet.Cells["A1"].PutValue("Sample Data");
sourceSheet.Cells["A2"].PutValue(100);
sourceSheet.Cells["A3"].PutValue(200);
// Create a destination workbook
Workbook destWorkbook = new Workbook();
// Copy theme from source workbook using Worksheet.Workbook property
destWorkbook.CopyTheme(sourceSheet.Workbook);
// Access destination worksheet and copy data
Worksheet destSheet = destWorkbook.Worksheets[0];
Aspose.Cells.Range sourceRange = sourceSheet.Cells.CreateRange("A1:A3");
Aspose.Cells.Range destRange = destSheet.Cells.CreateRange("A1:A3");
// Copy data with formatting
destRange.Copy(sourceRange);
// Save the destination workbook
destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Workbook](../../workbook/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
