##PivotField.Items
PivotField property. Get all labels of pivot items in this field
## PivotField.Items property
Get all labels of pivot items in this field.
```csharp
public string[] Items { get; }
```
### Examples
```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyItemsDemo
{
public static void Run()
{
// Create a workbook and add sample data
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
int index = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add pivot field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
PivotField pivotField = pivotTable.RowFields[0];
// Demonstrate Items property
string[] items = pivotField.Items;
Console.WriteLine("Pivot Field Items:");
foreach (string item in items)
{
Console.WriteLine(item);
}
// Set current page item
ArrayList list = new ArrayList(items);
if (list.Contains("Apple"))
{
pivotField.CurrentPageItem = (short)list.IndexOf("Apple");
Console.WriteLine("Current page item set to: Apple");
}
pivotTable.CalculateData();
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
