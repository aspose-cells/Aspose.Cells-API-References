##Class DataModel
Aspose.Cells.DataModels.DataModel class. Represents the data model
## DataModel class
Represents the data model.
```csharp
public class DataModel
```
## Properties
| Name | Description |
| --- | --- |
| [Relationships](../../aspose.cells.datamodels/datamodel/relationships/) { get; } | Gets all relationships of the tables in the data model. |
| [Tables](../../aspose.cells.datamodels/datamodel/tables/) { get; } | Gets all tables in the data model. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.DataModels;
using System;
public class DataModelsClassDataModelDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the DataModel from the workbook instead of creating a new instance
DataModel dataModel = workbook.DataModel;
// Demonstrate accessing tables and relationships (read-only properties)
Console.WriteLine("Number of tables in DataModel: " + dataModel.Tables.Count);
Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);
// Note: Since Tables and Relationships are read-only collections,
// we can only access existing items but not modify them directly
// Save the workbook (DataModel is typically used internally by Aspose.Cells)
workbook.Save("DataModelDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)
