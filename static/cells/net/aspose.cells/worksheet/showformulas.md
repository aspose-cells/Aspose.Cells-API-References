##Worksheet.ShowFormulas
Worksheet property. Indicates whether to show formulas or their results
## Worksheet.ShowFormulas property
Indicates whether to show formulas or their results.
```csharp
public bool ShowFormulas { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyShowFormulasDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set formula in cell A1
worksheet.Cells["A1"].Formula = "=1+2+3";
// Initially show calculated value
worksheet.ShowFormulas = false;
Console.WriteLine("ShowFormulas OFF: " + worksheet.Cells["A1"].StringValue);
// Toggle to show formula text
worksheet.ShowFormulas = true;
Console.WriteLine("ShowFormulas ON: " + worksheet.Cells["A1"].StringValue);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
