##WarningInfo.ErrorObject
WarningInfo property. The error object
## WarningInfo.ErrorObject property
The error object.
```csharp
public object ErrorObject { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WarningInfoPropertyErrorObjectDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
int nameIndex = workbook.Worksheets.Names.Add("MyName");
workbook.Worksheets.Names[nameIndex].RefersTo = "=Sheet1!$A$1";
workbook.Settings.WarningCallback = new NameWarningCallback(workbook);
// Trigger name conflict by copying worksheet with names
workbook.Worksheets.AddCopy(sheet.Name);
}
private class NameWarningCallback : IWarningCallback
{
private readonly Workbook _workbook;
public NameWarningCallback(Workbook workbook) => _workbook = workbook;
public void Warning(WarningInfo warningInfo)
{
if (warningInfo.Type == ExceptionType.DefinedName)
{
int originalIndex = (int)warningInfo.ErrorObject;
Name originalName = _workbook.Worksheets.Names[originalIndex];
int newIndex = _workbook.Worksheets.Names.Add(originalName.Text + "_Copy");
_workbook.Worksheets.Names[newIndex].RefersTo = originalName.RefersTo;
warningInfo.CorrectedObject = newIndex;
}
}
}
}
}
```
### See Also
* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
