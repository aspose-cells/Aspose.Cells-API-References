##WorkbookDesigner.GetSmartMarkers
WorkbookDesigner method. Returns a collection of smart markers in a spreadsheet
## WorkbookDesigner.GetSmartMarkers method
Returns a collection of smart markers in a spreadsheet.
```csharp
public string[] GetSmartMarkers()
```
### Return Value
A collection of smart markers
### Remarks
A string array is created on every call. The array is sorted and duplicated values are removed.
### Examples
```csharp
using System;
using System.Data;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerMethodGetSmartMarkersDemo
{
public static void Run()
{
// Create a sample template file in memory
Workbook templateWorkbook = new Workbook();
Cells cells = templateWorkbook.Worksheets[0].Cells;
// Add smart markers to the template
cells["A1"].PutValue("&=COLORS_TIMES.COLORS");
cells["B1"].PutValue("&=COLORS_TIMES.TIMES");
// Save template to memory stream
MemoryStream templateStream = new MemoryStream();
templateWorkbook.Save(templateStream, SaveFormat.Xlsx);
// Initialize WorkbookDesigner with the template
WorkbookDesigner designer = new WorkbookDesigner();
designer.Workbook = new Workbook(templateStream);
// Get and display smart markers
string[] smartMarkers = designer.GetSmartMarkers();
Console.WriteLine("Found smart markers:");
foreach (string marker in smartMarkers)
{
Console.WriteLine(marker);
}
// Prepare data source
DataTable data = new DataTable("COLORS_TIMES");
data.Columns.Add("COLORS", typeof(string));
data.Columns.Add("TIMES", typeof(DateTime));
data.Rows.Add("red", DateTime.Now.AddDays(-1));
data.Rows.Add("yellow", DateTime.Now);
data.Rows.Add("green", DateTime.Now.AddDays(1));
// Set data source and process
designer.SetDataSource(data);
designer.Process();
// Save result
designer.Workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
