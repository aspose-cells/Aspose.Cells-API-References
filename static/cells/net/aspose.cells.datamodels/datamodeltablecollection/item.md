##DataModelTableCollection.Item
DataModelTableCollection property. Gets the data model table by position of the collection
## DataModelTableCollection indexer (1 of 2)
Gets the data model table by position of the collection.
```csharp
public DataModelTable this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The position of the collection. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.DataModels;
using Aspose.Cells.Tables;
using System;
public class DataModelTableCollectionPropertyItemDemo1
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for a table
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Jane");
// Create a table
int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[tableIndex];
table.DisplayName = "EmployeeTable";
// Access the DataModelTableCollection
DataModelTableCollection dataModelTables = workbook.DataModel.Tables;
// Demonstrate reading the Item property (indexer)
Console.WriteLine("Number of tables: " + dataModelTables.Count);
for (int i = 0; i < dataModelTables.Count; i++)
{
DataModelTable tableItem = dataModelTables[i]; // Using Item property
Console.WriteLine($"Table {i}: {tableItem.Name}");
}
// Add another table to demonstrate multiple items
worksheet.Cells["D1"].PutValue("DeptID");
worksheet.Cells["E1"].PutValue("Department");
worksheet.Cells["D2"].PutValue(101);
worksheet.Cells["E2"].PutValue("HR");
int secondTableIndex = worksheet.ListObjects.Add(3, 0, 1, 1, true);
worksheet.ListObjects[secondTableIndex].DisplayName = "DepartmentTable";
// Show updated collection
Console.WriteLine("\nAfter adding second table:");
for (int i = 0; i < dataModelTables.Count; i++)
{
Console.WriteLine($"Table {i}: {dataModelTables[i].Name}");
}
// Save the workbook
workbook.Save("DataModelTableCollectionItemIndexDemo.xlsx");
}
}
}
```
### See Also
* class [DataModelTable](../../datamodeltable/)
* class [DataModelTableCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)
## DataModelTableCollection indexer (2 of 2)
Gets the data model table by the name.
```csharp
public DataModelTable this[string name] { get; }
```
| Parameter | Description |
| --- | --- |
| name | The name of data model table. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.DataModels;
using Aspose.Cells.Tables;
using System;
public class DataModelTableCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Widget");
worksheet.Cells["B2"].PutValue(49.99);
int tableIndex = worksheet.ListObjects.Add(0, 0, 1, 1, true);
ListObject table = worksheet.ListObjects[tableIndex];
table.DisplayName = "InventoryTable";
DataModelTableCollection dataModelTables = workbook.DataModel.Tables;
DataModelTable dataModelTable = dataModelTables["InventoryTable"];
Console.WriteLine("Initial Table Name: " + dataModelTable.Name);
worksheet.ListObjects[0].DisplayName = "UpdatedInventory";
dataModelTable = dataModelTables["UpdatedInventory"];
Console.WriteLine("Updated Table Name: " + dataModelTable.Name);
workbook.Save("DataModelTableCollectionItemDemo.xlsx");
}
}
}
```
### See Also
* class [DataModelTable](../../datamodeltable/)
* class [DataModelTableCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)
