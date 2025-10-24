##ExternalConnection.ConnectionString
ExternalConnection property. The connection information string is used to make contact with an OLE DB or ODBC data source
## ExternalConnection.ConnectionString property
The connection information string is used to make contact with an OLE DB or ODBC data source.
```csharp
public virtual string ConnectionString { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;
namespace AsposeCellsExamples
{
public class ExternalConnectionPropertyConnectionStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(1500);
// Create a pivot table
int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Get the data connections
ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
// Display connection string if exists
if (connections.Length > 0)
{
Console.WriteLine("Connection String: " + connections[0].ConnectionString);
}
// Save the workbook
workbook.Save("PivotTableWithConnection.xlsx");
}
}
}
```
### See Also
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
