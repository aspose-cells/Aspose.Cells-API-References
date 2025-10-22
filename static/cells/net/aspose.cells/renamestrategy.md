##Enum RenameStrategy
Aspose.Cells.RenameStrategy enum. Strategy option for duplicate names of columns
## RenameStrategy enumeration
Strategy option for duplicate names of columns.
```csharp
public enum RenameStrategy
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Exception | `0` | Throws exception. |
| Digit | `1` | Named with digit. Duplicated names will become ...1, ...2, etc. |
| Letter | `2` | Named with letter.. Duplicated names will become ...A, ...B, etc. |
### Remarks
When processing data with headers, some scenarios require the headers to be no duplication for all columns. For example, when exporting data to a datatable and the header is required to be taken as datatable's column name, duplicated values of the header are invalid. For such kind of situations, user may determine how to handle them by specifying this strategy.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class RenameStrategyDemo
{
public static void RenameStrategyExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to the worksheet
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["A3"].PutValue("Jane");
worksheet.Cells["A4"].PutValue("John");
// Create ExportTableOptions and set the RenameStrategy
ExportTableOptions options = new ExportTableOptions
{
RenameStrategy = RenameStrategy.Digit // Use the Digit strategy for duplicate names
};
// Export the worksheet data to a DataTable
System.Data.DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 1, options);
// Display the DataTable content
foreach (System.Data.DataRow row in dataTable.Rows)
{
foreach (var item in row.ItemArray)
{
Console.Write(item + "\t");
}
Console.WriteLine();
}
// Save the workbook
workbook.Save("RenameStrategyExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
