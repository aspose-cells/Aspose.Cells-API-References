##WorksheetCollection.GetNamedRangesAndTables
WorksheetCollection method. Gets all predefined named ranges in the spreadsheet
## WorksheetCollection.GetNamedRangesAndTables method
Gets all pre-defined named ranges in the spreadsheet.
```csharp
public Range[] GetNamedRangesAndTables()
```
### Return Value
An array of Range objects.
Returns null if the named range does not exist.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodGetNamedRangesAndTablesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create some named ranges
worksheet.Cells.CreateRange("A1:B2").Name = "TestRange1";
worksheet.Cells.CreateRange("C3:D4").Name = "TestRange2";
// Get all named ranges and tables
Aspose.Cells.Range[] ranges = workbook.Worksheets.GetNamedRangesAndTables();
// Display information about the ranges
Console.WriteLine("Found {0} named ranges:", ranges.Length);
foreach (Aspose.Cells.Range range in ranges)
{
Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
}
}
}
}
```
### See Also
* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
