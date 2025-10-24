##PaginatedSaveOptions.IgnoreError
PaginatedSaveOptions property. Indicates if you need to hide the error while rendering. The error can be error in shape image chart rendering etc
## PaginatedSaveOptions.IgnoreError property
Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc.
```csharp
public bool IgnoreError { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertyIgnoreErrorDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data with potential formatting errors
worksheet.Cells["A1"].PutValue("Sample Data");
worksheet.Cells["A2"].PutValue(123);
worksheet.Cells["A3"].PutValue(DateTime.Now);
// Create PDF save options
PdfSaveOptions options = new PdfSaveOptions();
// Set IgnoreError to true to skip any conversion errors
options.IgnoreError = true;
// Save the workbook as PDF
workbook.Save("PaginatedSaveWithIgnoreError.pdf", options);
Console.WriteLine("PDF saved with IgnoreError enabled.");
}
}
}
```
### See Also
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
