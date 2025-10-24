##Worksheet.FirstVisibleColumn
Worksheet property. Represents first visible column index
## Worksheet.FirstVisibleColumn property
Represents first visible column index.
```csharp
public int FirstVisibleColumn { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyFirstVisibleColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Hide the first column (index 0)
worksheet.Cells.HideColumn(0);
// Get and display the first visible column index
Console.WriteLine("First visible column index: " + worksheet.FirstVisibleColumn);
// Save the workbook
workbook.Save("FirstVisibleColumnDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
