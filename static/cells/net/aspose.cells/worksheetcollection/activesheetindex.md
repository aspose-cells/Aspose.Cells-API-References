##WorksheetCollection.ActiveSheetIndex
WorksheetCollection property. Represents the index of active worksheet when the spreadsheet is opened
## WorksheetCollection.ActiveSheetIndex property
Represents the index of active worksheet when the spreadsheet is opened.
```csharp
public int ActiveSheetIndex { get; set; }
```
### Remarks
Sheet index is zero based.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertyActiveSheetIndexDemo
{
public static void Run()
{
// Create a new workbook with 3 worksheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Set the active sheet index to 1 (second sheet)
workbook.Worksheets.ActiveSheetIndex = 1;
// Verify the active sheet
Console.WriteLine("Active Sheet: " + workbook.Worksheets[workbook.Worksheets.ActiveSheetIndex].Name);
// Save the workbook
string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "ActiveSheetDemo.xlsx");
workbook.Save(outputPath);
Console.WriteLine("File saved to: " + outputPath);
}
}
}
```
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
