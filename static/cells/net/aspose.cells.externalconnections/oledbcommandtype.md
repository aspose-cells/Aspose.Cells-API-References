##Enum OLEDBCommandType
Aspose.Cells.ExternalConnections.OLEDBCommandType enum. Specifies the OLE DB command type
## OLEDBCommandType enumeration
Specifies the OLE DB command type.
```csharp
public enum OLEDBCommandType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | The command type is not specified. |
| CubeName | `1` | Specifies a cube name |
| SqlStatement | `2` | Specifies a SQL statement |
| TableName | `3` | Specifies a table name |
| DefaultInformation | `4` | Specifies that default information has been given, and it is up to the provider how to interpret. |
| WebBasedList | `5` | Specifies a query which is against a web based List Data Provider. |
| TableCollection | `6` | Specifies the table list. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class ExternalConnectionsClassOLEDBCommandTypeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Mary");
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Get the external connection
ExternalConnectionCollection connections = workbook.DataConnections;
ExternalConnection conn = connections[0];
// Demonstrate OLEDBCommandType usage
Console.WriteLine("Connection Name: " + conn.Name);
Console.WriteLine("Source Type: " + conn.SourceType);
Console.WriteLine("Command Type: " + conn.CommandType);
Console.WriteLine("Command: " + conn.Command);
// Change command type and demonstrate
conn.CommandType = OLEDBCommandType.TableName;
Console.WriteLine("\nAfter changing CommandType:");
Console.WriteLine("Command Type: " + conn.CommandType);
// Save the workbook
workbook.Save("OLEDBCommandTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)
