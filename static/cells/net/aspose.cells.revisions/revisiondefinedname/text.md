##RevisionDefinedName.Text
RevisionDefinedName property. Gets the text of the defined name
## RevisionDefinedName.Text property
Gets the text of the defined name.
```csharp
public string Text { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;
namespace AsposeCellsExamples
{
public class RevisionDefinedNamePropertyTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a defined name
int index = workbook.Worksheets.Names.Add("TestName");
Name name = workbook.Worksheets.Names[index];
name.RefersTo = "=Sheet1!$A$1";
// Modify the defined name to generate revision
name.RefersTo = "=Sheet1!$B$1";
// Save to file to generate revisions
workbook.Save("RevisionDefinedName.xlsx");
// Reopen the file to read revisions
Workbook revisionWorkbook = new Workbook("RevisionDefinedName.xlsx");
// Check revisions
foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
{
foreach (Revision rv in log.Revisions)
{
if (rv.Type == RevisionType.DefinedName)
{
RevisionDefinedName rdn = (RevisionDefinedName)rv;
Console.WriteLine("Defined Name Text: " + rdn.Text);
Console.WriteLine("Old Formula: " + rdn.OldFormula);
Console.WriteLine("New Formula: " + rdn.NewFormula);
}
}
}
}
}
}
```
### See Also
* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
