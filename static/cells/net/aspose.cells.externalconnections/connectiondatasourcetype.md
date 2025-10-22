##Enum ConnectionDataSourceType
Aspose.Cells.ExternalConnections.ConnectionDataSourceType enum. Specifies external database source type
## ConnectionDataSourceType enumeration
Specifies external database source type
```csharp
public enum ConnectionDataSourceType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| ODBCBasedSource | `1` | ODBC-based source |
| DAOBasedSource | `2` | DAO-based source |
| FileBasedDataBaseSource | `3` | File based database source |
| WebQuery | `4` | Web query |
| OLEDBBasedSource | `5` | OLE DB-based source |
| TextBasedSource | `6` | Text-based source |
| ADORecordSet | `7` | ADO record set |
| DSP | `8` | DSP |
| OLEDBDataModel | `100` | OLE DB data source created by the Spreadsheet Data Model. |
| DataFeedDataModel | `101` | Data feed data source created by the Spreadsheet Data Model. |
| WorksheetDataModel | `102` | Worksheet data source created by the Spreadsheet Data Model. |
| Table | `102` | Worksheet data source created by the Spreadsheet Data Model. |
| TextDataModel | `103` | Text data source created by the Spreadsheet Data Model. |
| Unknown | `255` | Text data source created by the Spreadsheet Data Model. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
namespace AsposeCellsExamples
{
public class ExternalConnectionsClassConnectionDataSourceTypeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data to worksheet
sheet.Cells["A1"].PutValue("Product");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["A2"].PutValue("Item1");
sheet.Cells["B2"].PutValue(1000);
sheet.Cells["A3"].PutValue("Item2");
sheet.Cells["B3"].PutValue(2000);
// Create a pivot table using the worksheet data
var pivotTable = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
// Get the connection and demonstrate ConnectionDataSourceType
var conn = sheet.PivotTables[0].GetSourceDataConnections()[0];
Console.WriteLine("Connection Name: " + conn.Name);
Console.WriteLine("Class Type: " + conn.ClassType);
Console.WriteLine("Source Type: " + conn.SourceType);
Console.WriteLine("Command: " + conn.Command);
// Save the workbook
workbook.Save("ExternalConnectionDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)
