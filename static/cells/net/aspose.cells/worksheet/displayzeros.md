##Worksheet.DisplayZeros
Worksheet property. True if zero values are displayed
## Worksheet.DisplayZeros property
True if zero values are displayed.
```csharp
public bool DisplayZeros { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyDisplayZerosDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Demonstrate DisplayZeros = true (default)
sheet.DisplayZeros = true;
Cell cell1 = sheet.Cells["A1"];
cell1.PutValue(0);
Console.WriteLine("DisplayZeros=true: " + cell1.StringValue);
// Demonstrate DisplayZeros = false
sheet.DisplayZeros = false;
Cell cell2 = sheet.Cells["A2"];
cell2.PutValue(0);
Console.WriteLine("DisplayZeros=false: " + cell2.StringValue);
// Show custom formatting with DisplayZeros
Style style = wb.CreateStyle();
style.Custom = "0.00;\"Zero\";\"Negative\"";
Cell cell3 = sheet.Cells["A3"];
cell3.PutValue(0);
cell3.SetStyle(style);
Console.WriteLine("Custom format with DisplayZeros=true: " + cell3.StringValue);
sheet.DisplayZeros = false;
Cell cell4 = sheet.Cells["A4"];
cell4.PutValue(0);
cell4.SetStyle(style);
Console.WriteLine("Custom format with DisplayZeros=false: " + cell4.StringValue);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
