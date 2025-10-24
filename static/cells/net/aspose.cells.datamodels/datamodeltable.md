##Class DataModelTable
Aspose.Cells.DataModels.DataModelTable class. Represents properties of a single table in spreadsheet data model
## DataModelTable class
Represents properties of a single table in spreadsheet data model.
```csharp
public class DataModelTable
```
## Properties
| Name | Description |
| --- | --- |
| [ConnectionName](../../aspose.cells.datamodels/datamodeltable/connectionname/) { get; } | Gets the connection name of the data model table. |
| [Id](../../aspose.cells.datamodels/datamodeltable/id/) { get; } | Gets the id of the data model table. |
| [Name](../../aspose.cells.datamodels/datamodeltable/name/) { get; } | Gets the name of the data model table. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.DataModels;
using Aspose.Cells.Tables;
using Aspose.Cells.Pivot;
using System;
public class DataModelsClassDataModelTableDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create a table
worksheet.Cells["A1"].PutValue("ProductID");
worksheet.Cells["B1"].PutValue("ProductName");
worksheet.Cells["A2"].PutValue(101);
worksheet.Cells["B2"].PutValue("Laptop");
worksheet.Cells["A3"].PutValue(102);
worksheet.Cells["B3"].PutValue("Monitor");
// Create a ListObject (table)
int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[tableIndex];
table.DisplayName = "ProductsTable";
// Access the DataModelTable
DataModelTable dataModelTable = workbook.DataModel.Tables[0];
// Display DataModelTable properties
Console.WriteLine("Data Model Table Properties:");
Console.WriteLine($"ID: {dataModelTable.Id}");
Console.WriteLine($"Name: {dataModelTable.Name}");
Console.WriteLine($"Connection Name: {dataModelTable.ConnectionName}");
// Create a pivot table using the DataModelTable
Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, "ProductName");
pivotTable.AddFieldToArea(PivotFieldType.Data, "ProductID");
// Save the workbook
workbook.Save("DataModelTableDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)
