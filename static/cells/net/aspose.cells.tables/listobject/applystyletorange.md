##ListObject.ApplyStyleToRange
ListObject method. Apply the table style to the range
## ListObject.ApplyStyleToRange method
Apply the table style to the range.
```csharp
public void ApplyStyleToRange()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectMethodApplyStyleToRangeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create a list object
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create a list object
int index = worksheet.ListObjects.Add("A1", "B3", true);
ListObject listObject = worksheet.ListObjects[index];
// Apply style to the range of the list object
listObject.ApplyStyleToRange();
// Verify the style was applied by checking a cell's foreground color
Style style = worksheet.Cells["A1"].GetStyle();
Console.WriteLine("Foreground color applied: " + style.ForegroundColor);
// Convert list object to range and verify
listObject.ConvertToRange();
Console.WriteLine("List objects count after conversion: " + worksheet.ListObjects.Count);
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
