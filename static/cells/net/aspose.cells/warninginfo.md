##Class WarningInfo
Aspose.Cells.WarningInfo class. Warning info
## WarningInfo class
Warning info
```csharp
public class WarningInfo
```
## Properties
| Name | Description |
| --- | --- |
| [CorrectedObject](../../aspose.cells/warninginfo/correctedobject/) { get; set; } | Gets and sets the corrected object. |
| [Description](../../aspose.cells/warninginfo/description/) { get; } | Get description of warning info. |
| [ErrorObject](../../aspose.cells/warninginfo/errorobject/) { get; } | The error object. |
| [Type](../../aspose.cells/warninginfo/type/) { get; } | Get warning type. |
| [WarningType](../../aspose.cells/warninginfo/warningtype/) { get; } | (**Obsolete.**) Get warning type. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassWarningInfoDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set warning callback
workbook.Settings.WarningCallback = new WarningHandler();
// Trigger different warning types
worksheet.Cells["A1"].PutValue("InvalidName"); // Will trigger DefinedName warning
worksheet.Cells["A2"].PutValue(DateTime.MaxValue); // May trigger other warnings
Console.WriteLine("Warning demo completed.");
}
}
public class WarningHandler : IWarningCallback
{
public void Warning(WarningInfo warningInfo)
{
switch (warningInfo.WarningType)
{
case WarningType.DuplicateDefinedName:
warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
Console.WriteLine($"DefinedName warning handled. Corrected to: {warningInfo.CorrectedObject}");
break;
case WarningType.FontSubstitution:
Console.WriteLine($"Font warning: {warningInfo.Description}");
break;
case WarningType.UnsupportedFileFormat:
Console.WriteLine($"File format warning: {warningInfo.Description}");
break;
case WarningType.IO:
Console.WriteLine($"IO warning: {warningInfo.Description}");
break;
case WarningType.InvalidData:
case WarningType.Limitation:
Console.WriteLine($"Warning: {warningInfo.Description}");
break;
default:
Console.WriteLine($"Unknown warning type: {warningInfo.Description}");
break;
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
