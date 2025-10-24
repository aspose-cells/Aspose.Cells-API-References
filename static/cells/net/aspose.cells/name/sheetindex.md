##Name.SheetIndex
Name property. Indicates this name belongs to Workbook or Worksheet. 0  Global name otherwise index to sheet onebased
## Name.SheetIndex property
Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based)
```csharp
public int SheetIndex { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NamePropertySheetIndexDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some worksheets
workbook.Worksheets.Add("Sheet1");
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Create a named range in Sheet2
Worksheet sheet2 = workbook.Worksheets["Sheet2"];
int index = workbook.Worksheets.Names.Add("MyNamedRange");
Name name = workbook.Worksheets.Names[index];
name.RefersTo = "=Sheet2!$A$1:$B$10";
// Display the sheet index of the named range
Console.WriteLine("Sheet index of named range: " + name.SheetIndex);
// Save the workbook
workbook.Save("NamedRangeDemo.xlsx");
}
}
}
```
### See Also
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
