##PivotItem.GetStringValue
PivotItem method. Gets the string value of the pivot item If the value is null it will return
## PivotItem.GetStringValue method
Gets the string value of the pivot item If the value is null, it will return ""
```csharp
public string GetStringValue()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotItemMethodGetStringValueDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("example.xlsx");
// Access the first worksheet and pivot table
Worksheet worksheet = workbook.Worksheets[0];
PivotTable pivotTable = worksheet.PivotTables[0];
// Get the first row field and its pivot items
PivotField rowField = pivotTable.RowFields[0];
PivotItemCollection pivotItems = rowField.PivotItems;
// Demonstrate GetStringValue() method
string itemValue = pivotItems[1].GetStringValue();
Console.WriteLine("PivotItem value: " + itemValue);
// Save the modified workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
