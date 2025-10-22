##Workbook.AcceptAllRevisions
Workbook method. Accepts all tracked changes in the workbook
## Workbook.AcceptAllRevisions method
Accepts all tracked changes in the workbook.
```csharp
public void AcceptAllRevisions()
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodAcceptAllRevisionsDemo
{
public static void Run()
{
// Create a workbook with revisions
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some revisions (track changes must be enabled in Excel first)
worksheet.Cells["A1"].PutValue("Original Value");
// Save with revisions
string sourcePath = "source_with_revisions.xlsx";
workbook.Save(sourcePath, SaveFormat.Xlsx);
// Reopen the workbook
workbook = new Workbook(sourcePath);
// Check if has revisions and accept them
if (workbook.HasRevisions)
{
Console.WriteLine("Workbook has revisions. Accepting all...");
workbook.AcceptAllRevisions();
// Save without revisions
string destPath = "output_no_revisions.xlsx";
workbook.Save(destPath, SaveFormat.Xlsx);
Console.WriteLine("Revisions accepted and saved to: " + destPath);
}
else
{
Console.WriteLine("Workbook has no revisions.");
}
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
