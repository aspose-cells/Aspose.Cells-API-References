##Class RevisionCellChange
Aspose.Cells.Revisions.RevisionCellChange class. Represents the revision that changing cells
## RevisionCellChange class
Represents the revision that changing cells.
```csharp
public class RevisionCellChange : Revision
```
## Properties
| Name | Description |
| --- | --- |
| [CellName](../../aspose.cells.revisions/revisioncellchange/cellname/) { get; } | Gets the name of the cell. |
| [Column](../../aspose.cells.revisions/revisioncellchange/column/) { get; } | Gets the column index of the cell. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Gets the number of this revision.(Inherited from [`Revision`](../revision/).) |
| [IsNewFormatted](../../aspose.cells.revisions/revisioncellchange/isnewformatted/) { get; } | Indicates whether this cell is new formatted. |
| [IsOldFormatted](../../aspose.cells.revisions/revisioncellchange/isoldformatted/) { get; } | Indicates whether this cell is old formatted. |
| [NewFormula](../../aspose.cells.revisions/revisioncellchange/newformula/) { get; } | Gets the old formula. |
| [NewStyle](../../aspose.cells.revisions/revisioncellchange/newstyle/) { get; } | Gets the new style of the cell. |
| [NewValue](../../aspose.cells.revisions/revisioncellchange/newvalue/) { get; } | Gets new value of the cell. |
| [OldFormula](../../aspose.cells.revisions/revisioncellchange/oldformula/) { get; } | Gets the old formula. |
| [OldStyle](../../aspose.cells.revisions/revisioncellchange/oldstyle/) { get; } | Gets the old style of the cell. |
| [OldValue](../../aspose.cells.revisions/revisioncellchange/oldvalue/) { get; } | Gets old value of the cell. |
| [Row](../../aspose.cells.revisions/revisioncellchange/row/) { get; } | Gets the row index of the cell. |
| override [Type](../../aspose.cells.revisions/revisioncellchange/type/) { get; } | Represents the type of revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Gets the worksheet.(Inherited from [`Revision`](../revision/).) |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;
namespace AsposeCellsExamples
{
public class RevisionsClassRevisionCellChangeDemo
{
public static void Run()
{
// Create output directory if it doesn't exist
string outputDir = "output/";
System.IO.Directory.CreateDirectory(outputDir);
string filePath = outputDir + "RevisionsClassRevisionCellChangeDemo_out.xlsx";
// Create initial workbook and enable sharing
Workbook workbook = new Workbook();
workbook.Settings.Shared = true;
workbook.Save(filePath, SaveFormat.Xlsx);
// Reopen workbook to make tracked changes
Workbook workbook2 = new Workbook(filePath);
Worksheet sheet = workbook2.Worksheets[0];
// First revision: Set initial values
sheet.Cells["A1"].PutValue("Initial Value");
sheet.Cells["B2"].PutValue(100);
workbook2.Save(filePath, SaveFormat.Xlsx);
// Second revision: Modify values
sheet.Cells["A1"].PutValue("Updated Value");
sheet.Cells["B2"].PutValue(200);
workbook2.Save(filePath, SaveFormat.Xlsx);
// Load workbook to access revision logs
Workbook workbook3 = new Workbook(filePath);
// Process all revision logs
foreach (RevisionLog log in workbook3.Worksheets.RevisionLogs)
{
foreach (Revision rev in log.Revisions)
{
if (rev.Type == RevisionType.ChangeCells)
{
RevisionCellChange rcc = (RevisionCellChange)rev;
Console.WriteLine($"Revision Type: {rev.Type}");
Console.WriteLine($"Cell: {rcc.CellName} (Row: {rcc.Row}, Column: {rcc.Column})");
Console.WriteLine($"Old Value: {rcc.OldValue ?? "null"}");
Console.WriteLine($"New Value: {rcc.NewValue ?? "null"}");
Console.WriteLine("------------------------------------");
}
}
}
}
}
}
```
### See Also
* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)
