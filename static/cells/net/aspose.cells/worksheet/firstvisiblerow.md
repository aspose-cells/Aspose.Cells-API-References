##Worksheet.FirstVisibleRow
Worksheet property. Represents first visible row index
## Worksheet.FirstVisibleRow property
Represents first visible row index.
```csharp
public int FirstVisibleRow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyFirstVisibleRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set some sample data
for (int i = 0; i < 50; i++)
{
worksheet.Cells[i, 0].Value = "Row " + (i + 1);
}
// Set the first visible row to row 20
worksheet.FirstVisibleRow = 20;
// Display the first visible row
Console.WriteLine("First visible row: " + worksheet.FirstVisibleRow);
// Save the workbook
workbook.Save("FirstVisibleRowDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
