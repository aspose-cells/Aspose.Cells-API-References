##CopyOptions.CopyOptions
CopyOptions constructor. CopyOptions constructor
## CopyOptions constructor
CopyOptions constructor.
```csharp
public CopyOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CopyOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and get the first worksheet
Worksheet sourceSheet = workbook.Worksheets[0];
Worksheet destSheet = workbook.Worksheets[workbook.Worksheets.Add()];
// Add sample data to source sheet
sourceSheet.Cells["A1"].PutValue("Source Data");
sourceSheet.Cells["A2"].PutValue(100);
sourceSheet.Cells["A3"].PutValue(200);
sourceSheet.Cells["A4"].PutValue(300);
// Create CopyOptions using constructor
CopyOptions options = new CopyOptions();
options.ReferToDestinationSheet = true;
// Copy rows with the options
destSheet.Cells.CopyRows(sourceSheet.Cells, 0, 0, sourceSheet.Cells.MaxDisplayRange.RowCount, options);
// Save the workbook
workbook.Save("CopyOptionsDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
