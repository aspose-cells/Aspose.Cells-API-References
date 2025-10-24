##Enum RevisionActionType
Aspose.Cells.Revisions.RevisionActionType enum. Represents the type of revision action
## RevisionActionType enumeration
Represents the type of revision action.
```csharp
public enum RevisionActionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Add | `0` | Add revision. |
| Delete | `1` | Delete revision. |
| DeleteColumn | `2` | Column delete revision. |
| DeleteRow | `3` | Row delete revision. |
| InsertColumn | `4` | Column insert revision. |
| InsertRow | `5` | Row insert revision. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionsClassRevisionActionTypeDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Perform various operations that generate different revision types
worksheet.Cells["A1"].PutValue("Initial Value");
worksheet.Cells.InsertRow(0);
worksheet.Cells.DeleteRow(1);
worksheet.Cells.InsertColumn(0);
worksheet.Cells.DeleteColumn(1);
// Check if workbook has revisions
if (workbook.HasRevisions)
{
// Note: The original API doesn't provide direct access to revisions collection
// So we'll just demonstrate the RevisionActionType enum as requested
Console.WriteLine("Workbook contains revisions (but API doesn't provide access)");
}
// Demonstrate using RevisionActionType enum values
Console.WriteLine("Available revision action types:");
foreach (RevisionActionType actionType in Enum.GetValues(typeof(RevisionActionType)))
{
Console.WriteLine($"{actionType} = {(int)actionType}");
}
// Save the workbook
workbook.Save("RevisionActionTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)
