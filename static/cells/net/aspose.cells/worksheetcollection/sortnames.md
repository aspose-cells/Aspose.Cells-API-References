##WorksheetCollection.SortNames
WorksheetCollection method. Sorts the defined names
## WorksheetCollection.SortNames method
Sorts the defined names.
```csharp
public void SortNames()
```
### Remarks
If you create a large amount of named ranges in the Excel file, please call this method after all named ranges are created and before saving
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodSortNamesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some named ranges
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test1");
worksheet.Cells.CreateRange("A1").Name = "Range2";
worksheet.Cells["B1"].PutValue("Test2");
worksheet.Cells.CreateRange("B1").Name = "Range1";
// Display names before sorting
Console.WriteLine("Before sorting:");
foreach (Name name in workbook.Worksheets.Names)
{
Console.WriteLine(name.RefersTo);
}
// Sort the names
workbook.Worksheets.SortNames();
// Display names after sorting
Console.WriteLine("\nAfter sorting:");
foreach (Name name in workbook.Worksheets.Names)
{
Console.WriteLine(name.RefersTo);
}
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
