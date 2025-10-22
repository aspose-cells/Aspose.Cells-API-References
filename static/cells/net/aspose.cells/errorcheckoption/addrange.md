##ErrorCheckOption.AddRange
ErrorCheckOption method. Adds one influenced range by this setting
## ErrorCheckOption.AddRange method
Adds one influenced range by this setting.
```csharp
public int AddRange(CellArea ca)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | the range to be added. |
### Return Value
the index of the added range in the range list of this setting.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ErrorCheckOptionMethodAddRangeWithCellAreaDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;
int index = optsCollection.Add();
ErrorCheckOption opts = optsCollection[index];
opts.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
// Add ranges using CellArea
opts.AddRange(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 3 }); // A1:D2
opts.AddRange(new CellArea { StartRow = 2, StartColumn = 0, EndRow = 2, EndColumn = 3 }); // A3:D3
// Save the workbook
workbook.Save("ErrorCheckOptionMethodAddRangeWithCellAreaDemo.xls");
Console.WriteLine("Workbook saved with error check options.");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
