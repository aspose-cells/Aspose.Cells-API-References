##DataModelTable.Id
DataModelTable property. Gets the id of the data model table
## DataModelTable.Id property
Gets the id of the data model table.
```csharp
public string Id { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.DataModels;
using Aspose.Cells.Tables;
using System;
public class DataModelTablePropertyIdDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create a table
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("Item 1");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Item 2");
// Create a ListObject (table)
int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[index];
// Get the DataModelTable (this is read-only in the workbook)
DataModelTable dataModelTable = workbook.DataModel.Tables[0];
// Display the current Id value
Console.WriteLine("Current DataModelTable Id: " + dataModelTable.Id);
// Note: The Id property is read-only, so we cannot set it
// This demonstrates how to access and use the existing Id
// Example usage: Compare table IDs when working with multiple tables
DataModelTable secondTable = null;
if (workbook.DataModel.Tables.Count > 1)
{
secondTable = workbook.DataModel.Tables[1];
if (dataModelTable.Id != secondTable.Id)
{
Console.WriteLine("Different table IDs detected");
}
}
// Save the workbook
workbook.Save("DataModelTableIdDemo.xlsx");
}
}
}
```
### See Also
* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)
