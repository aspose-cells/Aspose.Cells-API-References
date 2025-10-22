##PivotTable.ShowInOutlineForm
PivotTable method. Layouts the PivotTable in outline form
## PivotTable.ShowInOutlineForm method
Layouts the PivotTable in outline form.
```csharp
public void ShowInOutlineForm()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodShowInOutlineFormDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Add sample data worksheet
Worksheet dataSheet = workbook.Worksheets[0];
dataSheet.Name = "Data";
// Add sample data
dataSheet.Cells["A1"].PutValue("Date");
dataSheet.Cells["B1"].PutValue("Product");
dataSheet.Cells["C1"].PutValue("Sales");
dataSheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
dataSheet.Cells["B2"].PutValue("Apple");
dataSheet.Cells["C2"].PutValue(1000);
dataSheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2));
dataSheet.Cells["B3"].PutValue("Banana");
dataSheet.Cells["C3"].PutValue(2000);
dataSheet.Cells["A4"].PutValue(new DateTime(2023, 1, 3));
dataSheet.Cells["B4"].PutValue("Apple");
dataSheet.Cells["C4"].PutValue(1500);
// Create pivot table worksheet
Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
// Add pivot table and get the reference
int pivotIndex = pivotSheet.PivotTables.Add(
"=Data!A1:C4",
"A3",
"PivotTable1");
PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
// Add fields to areas
pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
pivotTable.AddFieldToArea(PivotFieldType.Column, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Show in outline form
pivotTable.ShowInOutlineForm();
// Refresh and calculate data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableOutlineFormDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
