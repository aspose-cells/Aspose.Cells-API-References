##WarningInfo.Type
WarningInfo property. Get warning type
## WarningInfo.Type property
Get warning type.
```csharp
public ExceptionType Type { get; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WarningInfoPropertyTypeDemo
{
private class CustomWarningCallback : IWarningCallback
{
public void Warning(WarningInfo warningInfo)
{
if (warningInfo.Type == ExceptionType.DefinedName)
{
warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
Console.WriteLine($"Corrected object: {warningInfo.CorrectedObject}");
}
}
}
public static void Run()
{
using (var workbook = new Workbook())
{
workbook.Worksheets.Add("Sheet1");
int nameIndex = workbook.Worksheets.Names.Add("TestName");
Name name = workbook.Worksheets.Names[nameIndex];
name.RefersTo = "=Sheet1!$A$1";
using (var stream = new MemoryStream())
{
workbook.Save(stream, SaveFormat.Xlsx);
var loadOptions = new LoadOptions { WarningCallback = new CustomWarningCallback() };
new Workbook(stream, loadOptions);
}
}
}
}
}
```
### See Also
* enum [ExceptionType](../../exceptiontype/)
* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
