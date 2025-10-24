##Cells.IsDefaultRowHidden
Cells property. Indicates whether the row is default hidden
## Cells.IsDefaultRowHidden property
Indicates whether the row is default hidden.
```csharp
public bool IsDefaultRowHidden { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyIsDefaultRowHiddenDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set default row hidden property
worksheet.Cells.IsDefaultRowHidden = true;
// Display the current value of IsDefaultRowHidden
Console.WriteLine("IsDefaultRowHidden: " + worksheet.Cells.IsDefaultRowHidden);
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
