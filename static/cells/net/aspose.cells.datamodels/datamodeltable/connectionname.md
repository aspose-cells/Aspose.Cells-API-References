##DataModelTable.ConnectionName
DataModelTable property. Gets the connection name of the data model table
## DataModelTable.ConnectionName property
Gets the connection name of the data model table.
```csharp
public string ConnectionName { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.DataModels;
using Aspose.Cells.Tables;
using Aspose.Cells.Pivot;
using System;
public class DataModelTablePropertyConnectionNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create a table
worksheet.Cells["A1"].PutValue("OrderID");
worksheet.Cells["B1"].PutValue("Customer");
worksheet.Cells["A2"].PutValue(1001);
worksheet.Cells["B2"].PutValue("John Doe");
worksheet.Cells["A3"].PutValue(1002);
worksheet.Cells["B3"].PutValue("Jane Smith");
// Create a ListObject (table)
int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[tableIndex];
table.DisplayName = "OrdersTable";
// Access the DataModelTable
DataModelTable dataModelTable = workbook.DataModel.Tables[0];
// Display the current ConnectionName value
Console.WriteLine("Current ConnectionName: " + dataModelTable.ConnectionName);
// Create a pivot table using the DataModelTable's connection
Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Customer");
pivotTable.AddFieldToArea(PivotFieldType.Data, "OrderID");
// Note: ConnectionName is read-only, so we can't set it
// This demonstrates how to use the existing connection name
if (!string.IsNullOrEmpty(dataModelTable.ConnectionName))
{
Console.WriteLine("This table is connected via: " + dataModelTable.ConnectionName);
}
// Save the workbook
workbook.Save("DataModelTableConnectionNameDemo.xlsx");
}
}
}
```
### See Also
* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)
