##PivotFieldCollection.Type
PivotFieldCollection property. Gets the PivotFields type
## PivotFieldCollection.Type property
Gets the PivotFields type.
```csharp
public PivotFieldType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFieldCollectionPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["B1"].Value = "Quantity";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["B3"].Value = 5;
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B4"].Value = 7;
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
PivotFieldCollection rowFields = pivotTable.RowFields;
// Display the type of the pivot field collection
Console.WriteLine("PivotFieldCollection Type: " + rowFields.Type);
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
PivotFieldCollection dataFields = pivotTable.DataFields;
// Display the type of the data field collection
Console.WriteLine("DataFields Type: " + dataFields.Type);
// Calculate data and refresh the pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the result
workbook.Save("PivotFieldCollectionTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
