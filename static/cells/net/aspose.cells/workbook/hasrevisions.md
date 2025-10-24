##Workbook.HasRevisions
Workbook property. Gets if the workbook has any tracked changes
## Workbook.HasRevisions property
Gets if the workbook has any tracked changes
```csharp
public bool HasRevisions { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyHasRevisionsDemo
{
public static void Run()
{
// Create a workbook with revisions
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Make a change that will create a revision
worksheet.Cells["A1"].PutValue("Original Value");
// Check if workbook has revisions
Console.WriteLine("Workbook has revisions: " + workbook.HasRevisions);
// Accept all revisions (if any)
if (workbook.HasRevisions)
{
workbook.AcceptAllRevisions();
}
// Check again after accepting revisions
Console.WriteLine("Workbook has revisions after accepting: " + workbook.HasRevisions);
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
