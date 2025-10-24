##Workbook.DataModel
Workbook property. Gets data model in the workbook
## Workbook.DataModel property
Gets data model in the workbook.
```csharp
public DataModel DataModel { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.DataModels;
namespace AsposeCellsExamples
{
public class WorkbookPropertyDataModelDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add sample data to worksheets to create a data model
Worksheet sheet1 = workbook.Worksheets[0];
sheet1.Cells["A1"].PutValue("DepartmentID");
sheet1.Cells["B1"].PutValue("DepartmentName");
sheet1.Cells["A2"].PutValue(1);
sheet1.Cells["B2"].PutValue("HR");
sheet1.Cells["A3"].PutValue(2);
sheet1.Cells["B3"].PutValue("IT");
Worksheet sheet2 = workbook.Worksheets.Add("Employees");
sheet2.Cells["A1"].PutValue("EmployeeID");
sheet2.Cells["B1"].PutValue("EmployeeName");
sheet2.Cells["C1"].PutValue("DepartmentID");
sheet2.Cells["A2"].PutValue(101);
sheet2.Cells["B2"].PutValue("John");
sheet2.Cells["C2"].PutValue(1);
sheet2.Cells["A3"].PutValue(102);
sheet2.Cells["B3"].PutValue("Alice");
sheet2.Cells["C3"].PutValue(2);
// Demonstrate DataModel property usage
Console.WriteLine("Data Model Relationships:");
foreach (DataModelRelationship rel in workbook.DataModel.Relationships)
{
Console.WriteLine($"Relationship: {rel.PrimaryKeyTable}.{rel.PrimaryKeyColumn} -> {rel.ForeignKeyTable}.{rel.ForeignKeyColumn}");
}
Console.WriteLine("\nData Model Tables:");
foreach (DataModelTable table in workbook.DataModel.Tables)
{
Console.WriteLine($"Table: {table.Name}");
}
// Save the workbook
workbook.Save("WorkbookWithDataModel.xlsx");
}
}
}
```
### See Also
* class [DataModel](../../../aspose.cells.datamodels/datamodel/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
