##PivotItem.IsFormula
PivotItem property. Indicates whether this pivot item is a calculated formula item
## PivotItem.IsFormula property
Indicates whether this pivot item is a calculated formula item.
```csharp
[Obsolete("Use PivotItem.IsCalculatedItem property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsFormula { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use PivotItem.IsCalculatedItem property instead. This property will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotItemPropertyIsFormulaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 20;
worksheet.Cells["B4"].Value = 30;
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Get the first pivot item
PivotField pivotField = pivotTable.RowFields[0];
PivotItem pivotItem = pivotField.PivotItems[0];
// Display the current IsFormula value (obsolete property)
Console.WriteLine("Current IsFormula value: " + pivotItem.IsFormula);
// Set a new value for IsFormula (obsolete property)
pivotItem.IsFormula = true;
// Demonstrate the effect - this would mark the pivot item as a formula item
Console.WriteLine("After setting IsFormula to true: " + pivotItem.IsFormula);
// Note: In real usage, you should use IsCalculatedItem instead as IsFormula is obsolete
Console.WriteLine("IsCalculatedItem (recommended property): " + pivotItem.IsCalculatedItem);
// Save the result
workbook.Save("PivotItemPropertyIsFormulaDemo.xlsx");
}
}
}
```
### See Also
* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
