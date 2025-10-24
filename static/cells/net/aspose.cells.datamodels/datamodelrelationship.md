##Class DataModelRelationship
Aspose.Cells.DataModels.DataModelRelationship class. Represents a single relationship in the spreadsheet data model
## DataModelRelationship class
Represents a single relationship in the spreadsheet data model.
```csharp
public class DataModelRelationship
```
## Properties
| Name | Description |
| --- | --- |
| [ForeignKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/foreignkeycolumn/) { get; } | Gets the name of the foreign key table column for this relationship. |
| [ForeignKeyTable](../../aspose.cells.datamodels/datamodelrelationship/foreignkeytable/) { get; } | Gets the name of the foreign key table for this relationship. |
| [PrimaryKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/primarykeycolumn/) { get; } | Gets the name of the primary key table column for this relationship. |
| [PrimaryKeyTable](../../aspose.cells.datamodels/datamodelrelationship/primarykeytable/) { get; } | Gets the name of the primary key table for this relationship. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.DataModels;
using System;
public class DataModelsClassDataModelRelationshipDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for demonstration
worksheet.Cells["A1"].PutValue("Orders");
worksheet.Cells["A2"].PutValue("OrderID");
worksheet.Cells["A3"].PutValue("CustomerID");
worksheet.Cells["A4"].PutValue("OrderDate");
worksheet.Cells["C1"].PutValue("Customers");
worksheet.Cells["C2"].PutValue("CustomerID");
worksheet.Cells["C3"].PutValue("CustomerName");
worksheet.Cells["C4"].PutValue("ContactName");
// This demonstrates accessing an existing relationship's properties
// In a real scenario, you would get this from the DataModel
DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];
if (relationship != null)
{
// Display relationship properties (read-only)
Console.WriteLine("Sample Data Model Relationship Properties:");
Console.WriteLine("Primary Key Table: " + relationship.PrimaryKeyTable);
Console.WriteLine("Primary Key Column: " + relationship.PrimaryKeyColumn);
Console.WriteLine("Foreign Key Table: " + relationship.ForeignKeyTable);
Console.WriteLine("Foreign Key Column: " + relationship.ForeignKeyColumn);
}
else
{
Console.WriteLine("No data model relationships found");
}
// Save the workbook
workbook.Save("DataModelRelationshipDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)
