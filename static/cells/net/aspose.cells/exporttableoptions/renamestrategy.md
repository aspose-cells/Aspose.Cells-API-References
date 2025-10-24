##ExportTableOptions.RenameStrategy
ExportTableOptions property. Strategy for duplicate names of columns
## ExportTableOptions.RenameStrategy property
Strategy for duplicate names of columns.
```csharp
public RenameStrategy RenameStrategy { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExportTableOptionsPropertyRenameStrategyDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["A3"].PutValue("Jane");
worksheet.Cells["A4"].PutValue("John");
ExportTableOptions options = new ExportTableOptions
{
RenameStrategy = RenameStrategy.Digit
};
System.Data.DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 1, options);
Console.WriteLine("Exported DataTable with Digit RenameStrategy:");
foreach (System.Data.DataRow row in dataTable.Rows)
{
Console.WriteLine(row[0]);
}
workbook.Save("RenameStrategyDemo.xlsx");
}
}
}
```
### See Also
* enum [RenameStrategy](../../renamestrategy/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
