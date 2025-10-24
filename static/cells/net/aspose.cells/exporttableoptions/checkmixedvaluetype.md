##ExportTableOptions.CheckMixedValueType
ExportTableOptions property. False Aspose.Cells will set the DataColumns type by the value type of the first row for performance. True Aspose.Cells will check whether the value type in the column are mixed before set the DataColumns type And the value type are mixed the DataColumns type will be string
## ExportTableOptions.CheckMixedValueType property
False, Aspose.Cells will set the DataColumn's type by the value type of the first row for performance. True, Aspose.Cells will check whether the value type in the column are mixed before set the DataColumn's type And the value type are mixed, the DataColumn's type will be string.
```csharp
public bool CheckMixedValueType { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExportTableOptionsPropertyCheckMixedValueTypeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add headers
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Value Date");
// Add sample data with mixed types
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue(DateTime.Now);
worksheet.Cells["A3"].PutValue(2.5);
worksheet.Cells["B3"].PutValue("2023-01-15");
worksheet.Cells["A4"].PutValue("3");
worksheet.Cells["B4"].PutValue(DateTime.Now.AddDays(1));
// Create export options with CheckMixedValueType enabled
ExportTableOptions options = new ExportTableOptions
{
CheckMixedValueType = true,
ExportColumnName = true
};
// Export data to DataTable
DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 2, options);
// Display results
Console.WriteLine("Columns: " + dataTable.Columns.Count);
Console.WriteLine("Rows: " + dataTable.Rows.Count);
Console.WriteLine("ID column type: " + dataTable.Columns["ID"].DataType);
Console.WriteLine("Value Date column type: " + dataTable.Columns["Value Date"].DataType);
}
}
}
```
### See Also
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
