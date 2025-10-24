##ReferredArea.ExternalFileName
ReferredArea property. Get the external file name if this is an external reference
## ReferredArea.ExternalFileName property
Get the external file name if this is an external reference.
```csharp
public string ExternalFileName { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ReferredAreaPropertyExternalFileNameDemo
{
public static void Run()
{
// Create a workbook with external reference
Workbook wb = new Workbook();
// Create a name that refers to an external workbook
int index = wb.Worksheets.Names.Add("RefExternalName");
wb.Worksheets.Names[index].RefersTo = "='[ExternalLinkSource.xlsx]Sheet1'!$A$1:$C$3";
// Get the referred area
ReferredArea ra = wb.Worksheets.Names["RefExternalName"].GetReferredAreas(false)[0];
// Demonstrate ExternalFileName property
Console.WriteLine("External File Name: " + ra.ExternalFileName);
Console.WriteLine("Sheet Name: " + ra.SheetName);
Console.WriteLine("Area: R" + ra.StartRow + "C" + ra.StartColumn +
" to R" + ra.EndRow + "C" + ra.EndColumn);
// Verify the external file name
if (!ra.ExternalFileName.EndsWith("ExternalLinkSource.xlsx"))
{
Console.WriteLine("Error: ExternalFileName should be ExternalLinkSource.xlsx");
}
}
}
}
```
### See Also
* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
