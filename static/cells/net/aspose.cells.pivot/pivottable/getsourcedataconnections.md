##PivotTable.GetSourceDataConnections
PivotTable method. Gets the external connection data sources
## PivotTable.GetSourceDataConnections method
Gets the external connection data sources.
```csharp
public ExternalConnection[] GetSourceDataConnections()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;
namespace AsposeCellsExamples
{
public class PivotTableMethodGetSourceDataConnectionsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(200);
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Get source data connections
ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
// Display connection information
if (connections.Length > 0)
{
ExternalConnection conn = connections[0];
Console.WriteLine("Connection Name: " + conn.Name);
Console.WriteLine("Class Type: " + conn.ClassType);
Console.WriteLine("Source Type: " + conn.SourceType);
Console.WriteLine("Command: " + conn.Command);
}
// Save the workbook
workbook.Save("PivotTableSourceConnections.xlsx");
}
}
}
```
### See Also
* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
