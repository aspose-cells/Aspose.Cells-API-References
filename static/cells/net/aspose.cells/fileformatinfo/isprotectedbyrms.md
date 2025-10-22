##FileFormatInfo.IsProtectedByRMS
FileFormatInfo property. Gets whether the file is protected by Microsoft Rights Management Server
## FileFormatInfo.IsProtectedByRMS property
Gets whether the file is protected by Microsoft Rights Management Server.
```csharp
public bool IsProtectedByRMS { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FileFormatInfoPropertyIsProtectedByRMSDemo
{
public static void Run()
{
// Example 1: Check if RMS protected Excel file is protected
FileFormatInfo info1 = FileFormatUtil.DetectFileFormat("DRMExcel_document.xls");
Console.WriteLine("Is file protected by RMS: " + info1.IsProtectedByRMS);
// Example 2: Check if regular Excel file is protected
FileFormatInfo info2 = FileFormatUtil.DetectFileFormat("upload_simple_1.xls");
Console.WriteLine("Is file protected by RMS: " + info2.IsProtectedByRMS);
}
}
}
```
### See Also
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
