##ExternalConnection.SourceType
ExternalConnection property. Gets or Sets the external connection DataSource type
## ExternalConnection.SourceType property
Gets or Sets the external connection DataSource type.
```csharp
public ConnectionDataSourceType SourceType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
namespace AsposeCellsExamples
{
public class ExternalConnectionPropertySourceTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and create a pivot table
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Product");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["A2"].PutValue("Apple");
sheet.Cells["B2"].PutValue(1000);
sheet.Cells["A3"].PutValue("Banana");
sheet.Cells["B3"].PutValue(2000);
// Create pivot table
int index = sheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];
// Get the external connection
ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
// Demonstrate SourceType property
Console.WriteLine("Connection Source Type: " + conn.SourceType);
// Modify connection properties
conn.Name = "TestConnection";
conn.SourceType = ConnectionDataSourceType.OLEDBDataModel;
// Output modified properties
Console.WriteLine("Modified Connection Name: " + conn.Name);
Console.WriteLine("Modified Source Type: " + conn.SourceType);
}
}
}
```
### See Also
* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
