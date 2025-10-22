##CopyOptions.CopyNames
CopyOptions property. Indicates whether copying the names
## CopyOptions.CopyNames property
Indicates whether copying the names.
```csharp
public bool CopyNames { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CopyOptionsPropertyCopyNamesDemo
{
public static void Run()
{
// Create a source workbook with named ranges
Workbook sourceWorkbook = new Workbook();
Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
// Create a named range in source workbook
sourceSheet.Cells["A1"].PutValue("Test Value");
int index = sourceWorkbook.Worksheets.Names.Add("SourceName");
sourceWorkbook.Worksheets.Names[index].RefersTo = "=Sheet1!$A$1";
// Create a destination workbook
Workbook destWorkbook = new Workbook();
// Copy worksheet with CopyNames=true
destWorkbook.Worksheets[0].Copy(sourceSheet, new CopyOptions { CopyNames = true });
// Verify the named range was copied
Name copiedName = destWorkbook.Worksheets.Names["SourceName"];
if (copiedName != null)
{
Console.WriteLine("Named range copied successfully: " + copiedName.RefersTo);
}
else
{
Console.WriteLine("Named range was not copied");
}
}
}
}
```
### See Also
* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
