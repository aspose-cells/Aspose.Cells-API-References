##PivotItemCollection.GetEnumerator
PivotItemCollection method. Gets an enumerator over the elements in this collection in proper sequence
## PivotItemCollection.GetEnumerator method
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
public class PivotItemCollectionMethodGetEnumeratorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
// Get pivot field and its items
PivotField pivotField = pivotTable.RowFields[0];
PivotItemCollection pivotItems = pivotField.PivotItems;
try
{
// Call GetEnumerator method
IEnumerator enumerator = pivotItems.GetEnumerator();
Console.WriteLine("Pivot Items:");
while (enumerator.MoveNext())
{
PivotItem item = (PivotItem)enumerator.Current;
Console.WriteLine(item.Value);
}
// Save the workbook
workbook.Save("PivotItemCollectionMethodGetEnumeratorDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
}
}
}
}
```
### See Also
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
