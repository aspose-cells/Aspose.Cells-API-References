##WarningInfo.CorrectedObject
WarningInfo property. Gets and sets the corrected object
## WarningInfo.CorrectedObject property
Gets and sets the corrected object.
```csharp
public object CorrectedObject { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WarningInfoPropertyCorrectedObjectDemo
{
public static void Run()
{
// Create a workbook and trigger a warning
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set a name that would normally trigger a warning
string originalName = "MyRange";
worksheet.Cells.CreateRange(originalName);
// Handle warning callback
workbook.Settings.WarningCallback = new WarningHandler();
// This operation would trigger the warning callback
worksheet.Cells.CreateRange(originalName); // Duplicate range name
}
}
public class WarningHandler : IWarningCallback
{
public void Warning(WarningInfo warningInfo)
{
if (warningInfo.WarningType == WarningType.DuplicateDefinedName)
{
// Demonstrate CorrectedObject usage
warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
Console.WriteLine($"Warning handled. Original: {warningInfo.ErrorObject}, Corrected: {warningInfo.CorrectedObject}");
}
}
}
}
```
### See Also
* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
