##Style.Update
Style method. Apply the named style to the styles of the cells which use this named style. It works like clicking the ok button after you finished modifying the style. Only applies for named style
## Style.Update method
Apply the named style to the styles of the cells which use this named style. It works like clicking the "ok" button after you finished modifying the style. Only applies for named style.
```csharp
public void Update()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleMethodUpdateDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a style
Style style = workbook.CreateStyle();
style.Number = 3; // Set to Percent format
// Apply the style to cell A1
worksheet.Cells["A1"].SetStyle(style);
// Modify the style
style.Number = 4; // Change to Currency format
// Update the style changes
style.Update();
// Verify the style was updated
Console.WriteLine("Cell A1 Number Format: " + worksheet.Cells["A1"].GetStyle().Number);
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
