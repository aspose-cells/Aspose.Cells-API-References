##PivotFieldCollection.GetEnumerator
PivotFieldCollection method. Gets an enumerator over the elements in this collection in proper sequence
## PivotFieldCollection.GetEnumerator method
Gets an enumerator over the elements in this collection in proper sequence.
```csharp
public IEnumerator GetEnumerator()
```
### Return Value
enumerator
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
using System.Collections;
public class PivotFieldCollectionMethodGetEnumeratorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["A2"].Value = "Laptop";
worksheet.Cells["B2"].Value = 1200;
worksheet.Cells["A3"].Value = "Phone";
worksheet.Cells["B3"].Value = 800;
worksheet.Cells["A4"].Value = "Tablet";
worksheet.Cells["B4"].Value = 600;
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
PivotFieldCollection rowFields = pivotTable.RowFields;
try
{
// Call the GetEnumerator method
IEnumerator enumerator = rowFields.GetEnumerator();
Console.WriteLine("Pivot Fields in Row Area:");
while (enumerator.MoveNext())
{
PivotField field = (PivotField)enumerator.Current;
Console.WriteLine($"- {field.Name}");
}
// Add data field and refresh pivot table
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
pivotTable.RefreshData();
pivotTable.CalculateData();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
}
// Save the result
workbook.Save("PivotFieldCollectionGetEnumeratorDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
