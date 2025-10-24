##ExternalConnection.CommandType
ExternalConnection property. Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider
## ExternalConnection.CommandType property
Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given, and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider.
```csharp
public virtual OLEDBCommandType CommandType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
namespace AsposeCellsExamples
{
public class ExternalConnectionPropertyCommandTypeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(1500);
// Create a pivot table
int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];
// Get the external connection
ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
// Demonstrate CommandType property
Console.WriteLine("Original CommandType: " + conn.CommandType);
// Change and show CommandType
conn.CommandType = Aspose.Cells.ExternalConnections.OLEDBCommandType.TableName;
Console.WriteLine("Modified CommandType: " + conn.CommandType);
// Save the workbook
workbook.Save("ExternalConnectionCommandTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
