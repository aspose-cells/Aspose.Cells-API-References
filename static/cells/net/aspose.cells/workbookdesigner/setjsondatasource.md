##WorkbookDesigner.SetJsonDataSource
WorkbookDesigner method. Set json string value as data source of smart markers
## WorkbookDesigner.SetJsonDataSource method
Set json string value as data source of smart markers.
```csharp
public void SetJsonDataSource(string name, string json)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the table. If the value of JSON represents an object,it coult be null. |
| json | String | The value of Json string. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerMethodSetJsonDataSourceWithStringStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample marker in cell A1
worksheet.Cells["A1"].PutValue("&=$DataSource.Name");
// Create workbook designer
WorkbookDesigner designer = new WorkbookDesigner();
designer.Workbook = workbook;
// Sample JSON data
string jsonData = "{\"Name\":\"John Doe\",\"Age\":30,\"City\":\"New York\"}";
// Set JSON data source
designer.SetJsonDataSource("DataSource", jsonData);
// Process the markers
designer.Process();
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
