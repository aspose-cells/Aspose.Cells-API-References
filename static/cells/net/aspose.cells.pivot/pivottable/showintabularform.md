##PivotTable.ShowInTabularForm
PivotTable method. Layouts the PivotTable in tabular form
## PivotTable.ShowInTabularForm method
Layouts the PivotTable in tabular form.
```csharp
public void ShowInTabularForm()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodShowInTabularFormDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Add data worksheet
Worksheet dataSheet = workbook.Worksheets[0];
dataSheet.Name = "Data";
// Add sample data for pivot table
dataSheet.Cells["A1"].PutValue("Label");
dataSheet.Cells["B1"].PutValue("Value");
dataSheet.Cells["A2"].PutValue("A");
dataSheet.Cells["B2"].PutValue(10);
dataSheet.Cells["A3"].PutValue("B");
dataSheet.Cells["B3"].PutValue(20);
// Add pivot table sheet
Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
// Add pivot table
int pivotIndex = pivotSheet.PivotTables.Add("=Data!A1:B3", "A1", "PivotTable1");
PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
// Add fields to pivot table
int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Label");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Display pivot table in tabular form
pivotTable.ShowInTabularForm();
// Refresh and calculate pivot table data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableShowInTabularFormDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
