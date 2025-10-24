##Class ErrorCheckOption
Aspose.Cells.ErrorCheckOption class. Error check setting applied on certain ranges
## ErrorCheckOption class
Error check setting applied on certain ranges.
```csharp
public class ErrorCheckOption
```
## Methods
| Name | Description |
| --- | --- |
| [AddRange](../../aspose.cells/errorcheckoption/addrange/)(CellArea) | Adds one influenced range by this setting. |
| [GetCountOfRange](../../aspose.cells/errorcheckoption/getcountofrange/)() | Gets the count of ranges that influenced by this setting. |
| [GetRange](../../aspose.cells/errorcheckoption/getrange/)(int) | Gets the influenced range of this setting by given index. |
| [IsErrorCheck](../../aspose.cells/errorcheckoption/iserrorcheck/)(ErrorCheckType) | Checks whether given error type will be checked. |
| [RemoveRange](../../aspose.cells/errorcheckoption/removerange/)(int) | Removes one range by given index. |
| [SetErrorCheck](../../aspose.cells/errorcheckoption/seterrorcheck/)(ErrorCheckType, bool) | Sets whether given error type will be checked. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ErrorCheckOptionDemo
{
public static void ErrorCheckOptionExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the ErrorCheckOptionCollection from the worksheet
ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;
// Add a new ErrorCheckOption to the collection
int optionIdx = opts.Add();
ErrorCheckOption opt = opts[optionIdx];
// Set error check options
opt.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
opt.SetErrorCheck(ErrorCheckType.InconsistRange, false);
opt.SetErrorCheck(ErrorCheckType.TextDate, false);
opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
opt.SetErrorCheck(ErrorCheckType.Validation, false);
// Define a cell area and add it to the ErrorCheckOption
CellArea ca = CellArea.CreateCellArea("A1", "B10");
opt.AddRange(ca);
// Save the workbook
workbook.Save("ErrorCheckOptionExample.xlsx");
workbook.Save("ErrorCheckOptionExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
