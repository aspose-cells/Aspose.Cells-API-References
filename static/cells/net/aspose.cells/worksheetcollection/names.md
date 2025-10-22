##WorksheetCollection.Names
WorksheetCollection property. Gets the collection of all the Name objects in the spreadsheet
## WorksheetCollection.Names property
Gets the collection of all the Name objects in the spreadsheet.
```csharp
public NameCollection Names { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertyNamesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet with special characters in name
Worksheet worksheet = workbook.Worksheets.Add("My.Test");
// Access the Names collection
NameCollection names = workbook.Worksheets.Names;
// Add a new named range
int index = names.Add("My.Test!TestName");
Name namedRange = names[index];
// Set the range reference and demonstrate usage
namedRange.RefersTo = "=My.Test!$A$1:$B$2";
// Output the named range properties
Console.WriteLine("Name: " + namedRange.Text);
Console.WriteLine("FullText: " + namedRange.FullText);
Console.WriteLine("RefersTo: " + namedRange.RefersTo);
}
}
}
```
### See Also
* class [NameCollection](../../namecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
