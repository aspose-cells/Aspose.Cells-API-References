##ErrorCheckOption.SetErrorCheck
ErrorCheckOption method. Sets whether given error type will be checked
## ErrorCheckOption.SetErrorCheck method
Sets whether given error type will be checked.
```csharp
public void SetErrorCheck(ErrorCheckType errorCheckType, bool isCheck)
```
| Parameter | Type | Description |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | error type can be checked. |
| isCheck | Boolean | true if given error type needs to be checked(green triangle will be shown for cell if the check failed). |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ErrorCheckOptionMethodSetErrorCheckWithErrorCheckTypeBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("123");
worksheet.Cells["A2"].PutValue("Sample text for error checking");
// Configure error check options
ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;
int optionIndex = errorCheckOptions.Add();
ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];
// Demonstrate SetErrorCheck with different ErrorCheckType values
errorCheckOption.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, true);
errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
// Apply to entire worksheet
errorCheckOption.AddRange(CellArea.CreateCellArea(0, 0, worksheet.Cells.MaxRow, worksheet.Cells.MaxDataColumn));
workbook.Save("ErrorCheckExample.xlsx");
}
}
}
```
### See Also
* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
