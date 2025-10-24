##ReferredArea.IsExternalLink
ReferredArea property. Indicates whether this is an external link
## ReferredArea.IsExternalLink property
Indicates whether this is an external link.
```csharp
public bool IsExternalLink { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ReferredAreaPropertyIsExternalLinkDemo
{
public static void Run()
{
Workbook sourceWorkbook = new Workbook();
Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
Workbook externalWorkbook = new Workbook();
externalWorkbook.Worksheets[0].Cells["A1"].PutValue(100);
string externalFileName = "ExternalWorkbook.xlsx";
externalWorkbook.Save(externalFileName, SaveFormat.Xlsx);
sourceSheet.Cells["B1"].Formula = "=A1";
sourceSheet.Cells["B2"].Formula = "=['" + externalFileName + "']Sheet1!A1";
Cell cellB1 = sourceSheet.Cells["B1"];
ReferredAreaCollection areasB1 = cellB1.GetPrecedents();
Cell cellB2 = sourceSheet.Cells["B2"];
ReferredAreaCollection areasB2 = cellB2.GetPrecedents();
Console.WriteLine("Formula in B1: " + cellB1.Formula);
foreach (ReferredArea area in areasB1)
{
Console.WriteLine("Reference: " + area.ToString());
Console.WriteLine("IsExternalLink: " + area.IsExternalLink);
}
Console.WriteLine("\nFormula in B2: " + cellB2.Formula);
foreach (ReferredArea area in areasB2)
{
Console.WriteLine("Reference: " + area.ToString());
Console.WriteLine("IsExternalLink: " + area.IsExternalLink);
Console.WriteLine("ExternalFileName: " + area.ExternalFileName);
}
System.IO.File.Delete(externalFileName);
}
}
}
```
### See Also
* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
