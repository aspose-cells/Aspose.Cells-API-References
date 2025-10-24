##PivotTable.BaseFields
PivotTable property. Returns all base pivot fields in the PivotTable
## PivotTable.BaseFields property
Returns all base pivot fields in the PivotTable.
```csharp
public PivotFieldCollection BaseFields { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyBaseFieldsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["A5"].Value = "Apple";
worksheet.Cells["B1"].Value = "Quantity";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 15;
worksheet.Cells["B4"].Value = 20;
worksheet.Cells["B5"].Value = 5;
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Refresh pivot table data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Access BaseFields collection
PivotFieldCollection baseFields = pivotTable.BaseFields;
// Display original items from each base field
Console.WriteLine("Base Fields and their Original Items:");
foreach (PivotField field in baseFields)
{
Console.WriteLine($"Field: {field.Name}");
string[] originalItems = field.OriginalItems;
foreach (string item in originalItems)
{
Console.WriteLine($"- {item}");
}
}
}
}
}
```
### See Also
* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
