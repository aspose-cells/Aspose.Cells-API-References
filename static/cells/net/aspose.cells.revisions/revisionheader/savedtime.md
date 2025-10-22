##RevisionHeader.SavedTime
RevisionHeader property. Gets and sets rhe date and time when this set of revisions was saved
## RevisionHeader.SavedTime property
Gets and sets rhe date and time when this set of revisions was saved.
```csharp
public DateTime SavedTime { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionHeaderPropertySavedTimeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create a revision header instance
RevisionHeader revisionHeader = new RevisionHeader();
try
{
// Set the SavedTime property
revisionHeader.SavedTime = DateTime.Now;
// Get and display the SavedTime value
Console.WriteLine("SavedTime value: " + revisionHeader.SavedTime);
// Modify the SavedTime property
revisionHeader.SavedTime = DateTime.Now.AddHours(-1);
Console.WriteLine("Modified SavedTime value: " + revisionHeader.SavedTime);
// Save the workbook to demonstrate the property is being used
workbook.Save("SavedTimeDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
