##ErrorCheckOption.RemoveRange
ErrorCheckOption method. Removes one range by given index
## ErrorCheckOption.RemoveRange method
Removes one range by given index.
```csharp
public void RemoveRange(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the range to be removed. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ErrorCheckOptionMethodRemoveRangeWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;
// Create a new ErrorCheckOption and enable EmptyCellRef check
int optionIndex = errorCheckOptions.Add();
ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];
errorCheckOption.SetErrorCheck(ErrorCheckType.EmptyCellRef, true);
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 1;
area.EndColumn = 1;
int rangeIndex = errorCheckOption.AddRange(area);
int initialCount = errorCheckOption.GetCountOfRange();
try
{
errorCheckOption.RemoveRange(rangeIndex);
int finalCount = errorCheckOption.GetCountOfRange();
Console.WriteLine($"Ranges before removal: {initialCount}, after removal: {finalCount}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing RemoveRange: {ex.Message}");
}
workbook.Save("ErrorCheckOptionRemoveRangeDemo.xlsx");
}
}
}
```
### See Also
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
