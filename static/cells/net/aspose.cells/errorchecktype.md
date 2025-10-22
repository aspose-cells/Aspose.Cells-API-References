##Enum ErrorCheckType
Aspose.Cells.ErrorCheckType enum. Represents all error check type
## ErrorCheckType enumeration
Represents all error check type.
```csharp
public enum ErrorCheckType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| EvaluationError | `1` | Ignore errors when cells contain formulas that result in an error. |
| Calc | `1` |  |
| EmptyCellRef | `2` | Ignore errors when formulas refer to empty cells. |
| NumberStoredAsText | `4` | Ignore errors when numbers are formatted as text or are preceded by an apostrophe |
| TextNumber | `4` | Ignore errors when numbers are formatted as text or are preceded by an apostrophe |
| InconsistRange | `8` | Ignore errors when formulas omit certain cells in a region. |
| InconsistFormula | `16` | Ignore errors when a formula in a region of your worksheet differs from other formulas in the same region. |
| TwoDigitTextYear | `32` | Ignore errors when formulas contain text formatted cells with years represented as 2 digits. |
| TextDate | `32` | Ignore errors when formulas contain text formatted cells with years represented as 2 digits. |
| UnlockedFormula | `64` | Ignore errors when unlocked cells contain formulas. |
| UnproctedFormula | `64` | Ignore errors when unlocked cells contain formulas. |
| TableDataValidation | `128` | Ignore errors when a cell's value in a Table does not comply with the Data Validation rules specified. |
| Validation | `128` | Ignore errors when a cell's value in a Table does not comply with the Data Validation rules specified. |
| CalculatedColumn | `129` | Ignore errors when cells contain a value different from a calculated column formula. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ErrorCheckTypeDemo
{
public static void ErrorCheckTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access the ErrorCheckOptionCollection
ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;
// Add a new ErrorCheckOption
int optionIndex = errorCheckOptions.Add();
ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];
// Set various error check types to false
errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistRange, false);
errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, false);
errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
errorCheckOption.SetErrorCheck(ErrorCheckType.Validation, false);
// Define a cell area for the error check option
CellArea cellArea = CellArea.CreateCellArea("A1", "B10");
errorCheckOption.AddRange(cellArea);
// Save the workbook
workbook.Save("ErrorCheckTypeExample.xlsx");
workbook.Save("ErrorCheckTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
