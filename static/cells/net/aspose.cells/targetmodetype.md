##Enum TargetModeType
Aspose.Cells.TargetModeType enum. Represents the type of target mode
## TargetModeType enumeration
Represents the type of target mode.
```csharp
public enum TargetModeType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| External | `0` | External link |
| FilePath | `1` | Local and full paths to files or folders. |
| Email | `2` | Email. |
| CellReference | `3` | Link on cell or named range. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassTargetModeTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an external hyperlink
worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
// Get the hyperlink and check its TargetModeType
Hyperlink link = worksheet.Hyperlinks[0];
Console.WriteLine("Hyperlink TargetModeType: " + link.LinkType);
// Delete the hyperlink
link.Delete();
Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
