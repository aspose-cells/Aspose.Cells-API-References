##TableStyleElement.Type
TableStyleElement property. Gets the element type
## TableStyleElement.Type property
Gets the element type.
```csharp
public TableStyleElementType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class TableStyleElementPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create a table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Item1");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("Item2");
worksheet.Cells["B3"].PutValue(200);
// Create a table
int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[index];
table.TableStyleType = TableStyleType.TableStyleMedium9;
// Get the table style (using the style name instead of creating new one)
string styleName = table.TableStyleName;
TableStyle style = workbook.Worksheets.TableStyles[styleName];
// Access table style elements
TableStyleElement element = style.TableStyleElements[TableStyleElementType.HeaderRow];
// Display the current type of the element
Console.WriteLine("Current Type value: " + element.Type);
// Note: Type property is read-only, so we can't set it
// element.Type = TableStyleElementType.TotalRow; // This would cause compile error
// Demonstrate how different element types affect the table
Console.WriteLine("\nAvailable table style elements:");
foreach (TableStyleElementType type in Enum.GetValues(typeof(TableStyleElementType)))
{
try
{
TableStyleElement testElement = style.TableStyleElements[type];
Console.WriteLine($"Element type {type} exists in this style");
}
catch
{
Console.WriteLine($"Element type {type} not available in this style");
}
}
// Save the workbook
workbook.Save("TableStyleElementTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
