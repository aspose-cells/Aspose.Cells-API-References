##WarningInfo.WarningType
WarningInfo property. Get warning type
## WarningInfo.WarningType property
Get warning type.
```csharp
[Obsolete("Use WarningInfo.Type property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public WarningType WarningType { get; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use WarningInfo.Type property, instead. This property will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WarningInfoPropertyWarningTypeDemo
{
public static void Run()
{
// Create a workbook and trigger a warning
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// This will trigger a warning when saving with unsupported features
workbook.Settings.WarningCallback = new WarningCallback();
// Save with a format that might cause warnings
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
internal class WarningCallback : IWarningCallback
{
public void Warning(WarningInfo warningInfo)
{
// Demonstrate WarningType property usage
Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
// Handle specific warning types
if (warningInfo.WarningType == WarningType.UnsupportedFileFormat)
{
Console.WriteLine("Unsupported format warning detected!");
}
}
}
}
```
### See Also
* enum [WarningType](../../warningtype/)
* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
