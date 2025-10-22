##ExternalConnection.ClassType
ExternalConnection property. Gets the type of this ExternalConnection object
## ExternalConnection.ClassType property
Gets the type of this [`ExternalConnection`](../) object.
```csharp
public abstract ExternalConnectionClassType ClassType { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class ExternalConnectionPropertyClassTypeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Product");
sheet.Cells["B1"].PutValue("Sales");
for (int i = 2; i <= 10; i++)
{
sheet.Cells[$"A{i}"].PutValue($"Product {i-1}");
sheet.Cells[$"B{i}"].PutValue(i * 100);
}
// Create a pivot table with Data Model connection
int pivotIndex = sheet.PivotTables.Add("A1:B10", "C1", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Get the external connection and demonstrate ClassType property
ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
Console.WriteLine($"Connection ClassType: {conn.ClassType}");
Console.WriteLine($"Expected ClassType: {ExternalConnectionClassType.DataModel}");
// Save the workbook
workbook.Save("ExternalConnectionClassTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
