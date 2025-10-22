##PivotTable.ExternalConnectionDataSource
PivotTable property. Gets the external connection data source
## PivotTable.ExternalConnectionDataSource property
Gets the external connection data source.
```csharp
[Obsolete("Use PivotTable.GetSourceDataConnections() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ExternalConnection ExternalConnectionDataSource { get; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use PivotTable.GetSourceDataConnections() method. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;
namespace AsposeCellsExamples
{
public class PivotTablePropertyExternalConnectionDataSourceDemo
{
public static void Run()
{
// Create a workbook with external data connection
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Create sample data
sheet.Cells["A1"].PutValue("Product");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["A2"].PutValue("Apple");
sheet.Cells["B2"].PutValue(1000);
sheet.Cells["A3"].PutValue("Orange");
sheet.Cells["B3"].PutValue(2000);
// Add pivot table
int index = sheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
PivotTable pivot = sheet.PivotTables[index];
// Get the external connection (read-only property)
ExternalConnection connection = pivot.ExternalConnectionDataSource;
if (connection != null)
{
Console.WriteLine("Pivot table connection: " + connection.Name);
}
else
{
Console.WriteLine("No external connection found");
}
}
}
}
```
### See Also
* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
