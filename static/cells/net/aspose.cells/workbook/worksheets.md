##Workbook.Worksheets
Workbook property. Gets the WorksheetCollection collection in the spreadsheet
## Workbook.Worksheets property
Gets the [`WorksheetCollection`](../../worksheetcollection/) collection in the spreadsheet.
```csharp
public WorksheetCollection Worksheets { get; }
```
### Return Value
[`WorksheetCollection`](../../worksheetcollection/) collection
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyWorksheetsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Add a new worksheet
workbook.Worksheets.Add("SecondSheet");
// Access the second worksheet and add data
Worksheet secondSheet = workbook.Worksheets[1];
secondSheet.Cells["A1"].PutValue("Product");
secondSheet.Cells["B1"].PutValue("Price");
secondSheet.Cells["A2"].PutValue("Laptop");
secondSheet.Cells["B2"].PutValue(999.99);
// Save the workbook
workbook.Save("WorkbookWorksheetsDemo.xlsx");
// Output worksheet count
Console.WriteLine($"Number of worksheets: {workbook.Worksheets.Count}");
}
}
}
```
### See Also
* class [WorksheetCollection](../../worksheetcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
