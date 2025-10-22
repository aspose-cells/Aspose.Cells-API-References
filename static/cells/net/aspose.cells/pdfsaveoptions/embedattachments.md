##PdfSaveOptions.EmbedAttachments
PdfSaveOptions property. Indicates whether to embed attachment for Ole objects in Excel
## PdfSaveOptions.EmbedAttachments property
Indicates whether to embed attachment for Ole objects in Excel.
```csharp
public bool EmbedAttachments { get; set; }
```
### Remarks
Default value is false. The value must be false when PDF/A compliance is set or pdf encryption is enabled.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;
using System.IO;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsPropertyEmbedAttachmentsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("PDF with Embedded Attachments Example");
// Create a sample file to embed
string sampleFile = "sample.docx";
File.WriteAllText(sampleFile, "This is a sample document");
// Add an attachment (OLE object) to the worksheet
int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(sampleFile));
worksheet.OleObjects[oleIndex].FileFormatType = FileFormatType.Docx;
worksheet.OleObjects[oleIndex].DisplayAsIcon = true;
// Create PDF save options
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Set the EmbedAttachments property to true
pdfSaveOptions.EmbedAttachments = true;
// Save the workbook as PDF with embedded attachments
workbook.Save("PdfWithEmbeddedAttachments.pdf", pdfSaveOptions);
// Clean up
File.Delete(sampleFile);
}
}
}
```
### See Also
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
