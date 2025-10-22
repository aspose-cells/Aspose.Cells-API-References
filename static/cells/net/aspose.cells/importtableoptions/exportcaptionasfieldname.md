##ImportTableOptions.ExportCaptionAsFieldName
ImportTableOptions property. Indicates whether exporting caption as field name
## ImportTableOptions.ExportCaptionAsFieldName property
Indicates whether exporting caption as field name
```csharp
public bool ExportCaptionAsFieldName { get; set; }
```
### Remarks
Only works for DataTable.
### Examples
```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ImportTableOptionsPropertyExportCaptionAsFieldNameDemo
{
public class Transaction
{
public string orderId { get; set; }
public string paymentType { get; set; }
public string orderType { get; set; }
}
public static void Run()
{
// Create sample data
List<Transaction> transactions = new List<Transaction>
{
new Transaction { orderId = "w101", paymentType = "card", orderType = "bur" },
new Transaction { orderId = "w102", paymentType = "cash", orderType = "piz" },
new Transaction { orderId = "w103", paymentType = "card", orderType = "sal" }
};
// Create workbook and import data with ExportCaptionAsFieldName
Workbook workbook = new Workbook();
ImportTableOptions importOptions = new ImportTableOptions();
importOptions.ExportCaptionAsFieldName = true;
workbook.Worksheets[0].Cells.ImportCustomObjects(transactions, 0, 0, importOptions);
// Export data back to verify
ExportTableOptions exportOptions = new ExportTableOptions();
List<Transaction> exportedData = workbook.Worksheets[0].Cells.ExportList<Transaction>(0, 0, 5, 10, exportOptions);
// Output verification
Console.WriteLine($"Exported count: {exportedData.Count}");
Console.WriteLine($"First payment type: {exportedData[0].paymentType}");
}
}
}
```
### See Also
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
