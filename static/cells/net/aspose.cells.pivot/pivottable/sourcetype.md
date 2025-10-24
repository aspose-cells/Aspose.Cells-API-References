##PivotTable.SourceType
PivotTable property. Gets the data source type of the pivot table
## PivotTable.SourceType property
Gets the data source type of the pivot table.
```csharp
public PivotTableSourceType SourceType { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTablePropertySourceTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["B1"].Value = "Region";
worksheet.Cells["C1"].Value = "Sales";
worksheet.Cells["A2"].Value = "Product A";
worksheet.Cells["B2"].Value = "North";
worksheet.Cells["C2"].Value = 1000;
worksheet.Cells["A3"].Value = "Product B";
worksheet.Cells["B3"].Value = "South";
worksheet.Cells["C3"].Value = 2000;
worksheet.Cells["A4"].Value = "Product C";
worksheet.Cells["B4"].Value = "East";
worksheet.Cells["C4"].Value = 3000;
// Create a pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("=A1:C4", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Display the current SourceType value
Console.WriteLine("Current PivotTable SourceType: " + pivotTable.SourceType);
// Calculate data to show the pivot table
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableSourceTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotTableSourceType](../../pivottablesourcetype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
