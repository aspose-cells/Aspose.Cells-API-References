##Enum ExternalConnectionClassType
Aspose.Cells.ExternalConnections.ExternalConnectionClassType enum. Represents the type of connection
## ExternalConnectionClassType enumeration
Represents the type of connection
```csharp
public enum ExternalConnectionClassType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Database | `0` | ODBC or OLE DB |
| WebQuery | `1` | Web query |
| TextBased | `2` | Based on text |
| DataModel | `3` | Data model |
| Unkown | `4` |  |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class ExternalConnectionsClassExternalConnectionClassTypeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the connection
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
for (int i = 2; i <= 10; i++)
{
worksheet.Cells[$"A{i}"].PutValue(i - 1);
worksheet.Cells[$"B{i}"].PutValue($"Name_{i - 1}");
}
// Create a pivot table with the data
int pivotIndex = worksheet.PivotTables.Add("A1:B10", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Get the external connection and demonstrate properties
ExternalConnection conn = workbook.DataConnections[0];
Console.WriteLine($"Connection Name: {conn.Name}");
Console.WriteLine($"Class Type: {conn.ClassType}");
Console.WriteLine($"Source Type: {conn.SourceType}");
Console.WriteLine($"Command: {conn.Command}");
Console.WriteLine($"Connection File: {conn.ConnectionFile ?? "null"}");
Console.WriteLine($"Connection String: {conn.ConnectionString ?? "null"}");
}
}
}
```
### See Also
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)
