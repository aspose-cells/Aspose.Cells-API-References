##WorksheetCollection.ActiveSheetName
WorksheetCollection property. Represents the name of active worksheet when the spreadsheet is opened
## WorksheetCollection.ActiveSheetName property
Represents the name of active worksheet when the spreadsheet is opened.
```csharp
public string ActiveSheetName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertyActiveSheetNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some worksheets
workbook.Worksheets.Add("Sheet1");
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Set the active sheet by name
workbook.Worksheets.ActiveSheetName = "Sheet2";
// Verify the active sheet
Console.WriteLine("Active Sheet: " + workbook.Worksheets.ActiveSheetName);
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
