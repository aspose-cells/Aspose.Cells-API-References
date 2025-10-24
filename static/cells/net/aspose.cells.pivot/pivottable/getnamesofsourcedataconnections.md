##PivotTable.GetNamesOfSourceDataConnections
PivotTable method. Gets the name of external source data connections
## PivotTable.GetNamesOfSourceDataConnections method
Gets the name of external source data connections.
```csharp
public string[] GetNamesOfSourceDataConnections()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodGetNamesOfSourceDataConnectionsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].Value = "Product";
sheet.Cells["B1"].Value = "Sales";
sheet.Cells["A2"].Value = "A";
sheet.Cells["B2"].Value = 100;
sheet.Cells["A3"].Value = "B";
sheet.Cells["B3"].Value = 200;
// Create pivot table and get reference
int pivotIndex = sheet.PivotTables.Add("PivotTable", "A1:B3", "C1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
// Get source data connections
string[] connections = pivotTable.GetNamesOfSourceDataConnections();
// Output the connection information
Console.WriteLine("Pivot Table Source Data Connections:");
foreach (string connection in connections)
{
Console.WriteLine(connection);
}
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
