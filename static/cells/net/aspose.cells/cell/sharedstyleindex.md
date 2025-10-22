##Cell.SharedStyleIndex
Cell property. Gets cells shared style index in the style pool
## Cell.SharedStyleIndex property
Gets cell's shared style index in the style pool.
```csharp
public int SharedStyleIndex { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertySharedStyleIndexDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style and set some properties
Style style = workbook.CreateStyle();
style.Font.Name = "Arial";
style.Font.Size = 12;
style.Font.IsBold = true;
// Apply the style to cell A1
worksheet.Cells["A1"].SetStyle(style);
// Get the shared style index of cell A1
int sharedStyleIndex = worksheet.Cells["A1"].SharedStyleIndex;
// Retrieve the style from the style pool using the index
Style retrievedStyle = workbook.GetStyleInPool(sharedStyleIndex);
// Output style information to verify
Console.WriteLine("Font Name: " + retrievedStyle.Font.Name);
Console.WriteLine("Font Size: " + retrievedStyle.Font.Size);
Console.WriteLine("Is Bold: " + retrievedStyle.Font.IsBold);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
