##ExportTableOptions.FormatStrategy
ExportTableOptions property. Gets and sets the format strategy when exporting the value as string value
## ExportTableOptions.FormatStrategy property
Gets and sets the format strategy when exporting the value as string value.
```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExportTableOptionsPropertyFormatStrategyDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with formatting
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Laptop");
worksheet.Cells["B2"].PutValue(999.99);
Style styleB2 = worksheet.Cells["B2"].GetStyle();
styleB2.Number = 4; // Currency format
worksheet.Cells["B2"].SetStyle(styleB2);
worksheet.Cells["A3"].PutValue("Phone");
worksheet.Cells["B3"].PutValue(599.99);
Style styleB3 = worksheet.Cells["B3"].GetStyle();
styleB3.Number = 4; // Currency format
worksheet.Cells["B3"].SetStyle(styleB3);
// Create export options with different format strategies
ExportTableOptions optionsDisplayStyle = new ExportTableOptions
{
FormatStrategy = CellValueFormatStrategy.DisplayStyle,
ExportColumnName = true
};
ExportTableOptions optionsCellStyle = new ExportTableOptions
{
FormatStrategy = CellValueFormatStrategy.CellStyle,
ExportColumnName = true
};
// Export using different strategies
Console.WriteLine("DisplayStyle Format Strategy:");
DataTable dtDisplay = worksheet.Cells.ExportDataTable(0, 0, 3, 2, optionsDisplayStyle);
PrintDataTable(dtDisplay);
Console.WriteLine("\nCellStyle Format Strategy:");
DataTable dtCellStyle = worksheet.Cells.ExportDataTable(0, 0, 3, 2, optionsCellStyle);
PrintDataTable(dtCellStyle);
}
private static void PrintDataTable(DataTable dt)
{
foreach (DataRow row in dt.Rows)
{
foreach (var item in row.ItemArray)
{
Console.Write(item + "\t");
}
Console.WriteLine();
}
}
}
}
```
### See Also
* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
