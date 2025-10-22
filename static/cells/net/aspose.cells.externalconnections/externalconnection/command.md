##ExternalConnection.Command
ExternalConnection property. The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data
## ExternalConnection.Command property
The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data
```csharp
public virtual string Command { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ExternalConnectionPropertyCommandDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and some sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(150);
// Create a table range
var range = worksheet.Cells.CreateRange("A1:B3");
// Create a pivot table using the range as source
int index = worksheet.PivotTables.Add("D1", "A1:B3", "PivotTable1");
var pivotTable = worksheet.PivotTables[index];
// Get the external connections
ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
// Display the Command property of the connection
if (connections.Length > 0)
{
Console.WriteLine("Connection Command: " + connections[0].Command);
}
// Save the workbook
workbook.Save("ExternalConnectionCommandDemo.xlsx");
}
}
}
```
### See Also
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
