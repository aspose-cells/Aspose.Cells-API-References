##ErrorCheckOption.IsErrorCheck
ErrorCheckOption method. Checks whether given error type will be checked
## ErrorCheckOption.IsErrorCheck method
Checks whether given error type will be checked.
```csharp
public bool IsErrorCheck(ErrorCheckType errorCheckType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | error type can be checked |
### Return Value
return true if given error type will be checked(green triangle will be shown for cell if the check failed).
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ErrorCheckOptionMethodIsErrorCheckWithErrorCheckTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
int index = options.Add();
ErrorCheckOption option = options[index];
// Configure error check settings
option.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
option.SetErrorCheck(ErrorCheckType.EvaluationError, true);
option.SetErrorCheck(ErrorCheckType.InconsistRange, false);
// Add range to apply these settings
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 10;
area.StartColumn = 0;
area.EndColumn = 5;
option.AddRange(area);
// Verify and display the settings
Console.WriteLine("NumberStoredAsText check enabled: " +
option.IsErrorCheck(ErrorCheckType.NumberStoredAsText));
Console.WriteLine("EvaluationError check enabled: " +
option.IsErrorCheck(ErrorCheckType.EvaluationError));
Console.WriteLine("InconsistRange check enabled: " +
option.IsErrorCheck(ErrorCheckType.InconsistRange));
}
}
}
```
### See Also
* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
