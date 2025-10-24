##ErrorCheckOption.GetCountOfRange
ErrorCheckOption method. Gets the count of ranges that influenced by this setting
## ErrorCheckOption.GetCountOfRange method
Gets the count of ranges that influenced by this setting.
```csharp
public int GetCountOfRange()
```
### Return Value
the count of ranges that influenced by this setting.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ErrorCheckOptionMethodGetCountOfRangeDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Get error check options collection
ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;
// Add first error check option
int index1 = optsCollection.Add();
ErrorCheckOption opts1 = optsCollection[index1];
opts1.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
opts1.AddRange(CellArea.CreateCellArea("A1", "D2"));
opts1.AddRange(CellArea.CreateCellArea("A3", "D3"));
// Add second error check option
int index2 = optsCollection.Add();
ErrorCheckOption opts2 = optsCollection[index2];
opts2.SetErrorCheck(ErrorCheckType.TwoDigitTextYear, false);
opts2.AddRange(CellArea.CreateCellArea("A3", "D5"));
// Demonstrate GetCountOfRange method
Console.WriteLine("First option range count: " + opts1.GetCountOfRange());
Console.WriteLine("Second option range count: " + opts2.GetCountOfRange());
// Save the workbook
workbook.Save("ErrorCheckOptionDemo.xlsx");
}
}
}
```
### See Also
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
