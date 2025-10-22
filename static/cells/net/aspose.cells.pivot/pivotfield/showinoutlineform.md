##PivotField.ShowInOutlineForm
PivotField property. Indicates whether layout this field in outline form on the Pivot Table view
## PivotField.ShowInOutlineForm property
Indicates whether layout this field in outline form on the Pivot Table view
```csharp
public bool ShowInOutlineForm { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyShowInOutlineFormDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Apple";
worksheet.Cells["A4"].Value = "Orange";
worksheet.Cells["A5"].Value = "Orange";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 15;
worksheet.Cells["B4"].Value = 20;
worksheet.Cells["B5"].Value = 25;
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add row field and demonstrate ShowInOutlineForm
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
PivotField rowField = pivotTable.RowFields[0];
// Set ShowInOutlineForm to false
rowField.ShowInOutlineForm = false;
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Refresh and calculate pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldShowInOutlineFormDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
