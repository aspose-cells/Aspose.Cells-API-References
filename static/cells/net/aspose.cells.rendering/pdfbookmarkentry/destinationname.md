##PdfBookmarkEntry.DestinationName
PdfBookmarkEntry property. Gets or sets name of destination
## PdfBookmarkEntry.DestinationName property
Gets or sets name of destination.
```csharp
public string DestinationName { get; set; }
```
### Remarks
If destination name is set, the destination will be defined as a named destination with this name.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class PdfBookmarkEntryPropertyDestinationNameDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample content to cells
worksheet.Cells["A1"].PutValue("Primary Content Section");
worksheet.Cells["A2"].PutValue("Secondary Content Section");
// Create main PDF bookmark entry
PdfBookmarkEntry mainEntry = new PdfBookmarkEntry
{
Text = "Main Section",
Destination = worksheet.Cells["A1"],
IsOpen = true
};
// Demonstrate reading initial DestinationName (null)
Console.WriteLine($"Initial DestinationName: {mainEntry.DestinationName ?? "null"}");
// Set custom destination name for main entry
mainEntry.DestinationName = "PrimaryDestination";
Console.WriteLine($"Updated DestinationName: {mainEntry.DestinationName}");
// Create sub-bookmark entry
PdfBookmarkEntry subEntry = new PdfBookmarkEntry
{
Text = "Sub Section",
Destination = worksheet.Cells["A2"],
DestinationName = "SecondaryDestination"
};
// Add sub-entry to main bookmark
mainEntry.SubEntry = new System.Collections.ArrayList { subEntry };
// Configure PDF save options with bookmark structure
PdfSaveOptions pdfOptions = new PdfSaveOptions
{
Bookmark = mainEntry
};
// Save the workbook with PDF bookmarks
workbook.Save("PdfBookmarkDestinationDemo.pdf", pdfOptions);
Console.WriteLine("PDF created with custom bookmark destinations.");
}
}
}
```
### See Also
* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
