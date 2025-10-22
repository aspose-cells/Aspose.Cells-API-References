##PivotTable.GetChildren
PivotTable method. Gets the Children Pivot Tables which use this PivotTable data as data source
## PivotTable.GetChildren method
Gets the Children Pivot Tables which use this PivotTable data as data source.
```csharp
public PivotTable[] GetChildren()
```
### Return Value
the PivotTable array object
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodGetChildrenDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Product");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["B2"].PutValue(100);
sheet.Cells["A3"].PutValue("B");
sheet.Cells["B3"].PutValue(200);
sheet.Cells["A4"].PutValue("C");
sheet.Cells["B4"].PutValue(300);
// Create main pivot table
PivotTableCollection pivotTables = sheet.PivotTables;
int index = pivotTables.Add("A1:B4", "E3", "MainPivotTable");
PivotTable mainPivotTable = pivotTables[index];
mainPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
mainPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Create child pivot table
index = pivotTables.Add("A1:B4", "E10", "ChildPivotTable");
PivotTable childPivotTable = pivotTables[index];
childPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
childPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Establish relationship by sharing base fields
foreach (PivotField field in mainPivotTable.BaseFields)
{
childPivotTable.BaseFields.Add(field);
}
// Demonstrate GetChildren() method
Console.WriteLine("Child Pivot Tables:");
foreach (PivotTable child in mainPivotTable.GetChildren())
{
Console.WriteLine("Child Pivot Table Name: " + child.Name);
Console.WriteLine("Child Pivot Table Location: " + child.TableRange1);
}
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
