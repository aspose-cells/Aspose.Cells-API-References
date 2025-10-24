##PdfSaveOptions.CustomPropertiesExport
PdfSaveOptions property. Gets or sets a value determining the way CustomDocumentPropertyCollection are exported to PDF file. Default value is None
## PdfSaveOptions.CustomPropertiesExport property
Gets or sets a value determining the way [`CustomDocumentPropertyCollection`](../../../aspose.cells.properties/customdocumentpropertycollection/) are exported to PDF file. Default value is None.
```csharp
public PdfCustomPropertiesExport CustomPropertiesExport { get; set; }
```
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsPropertyCustomPropertiesExportDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello Aspose");
worksheet.Cells["A2"].PutValue("Sample PDF Export");
workbook.CustomDocumentProperties.Add("Author", "John Doe");
workbook.CustomDocumentProperties.Add("Subject", "Aspose.Cells Example");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;
workbook.Save("PdfCustomPropertiesExportDemo.pdf", saveOptions);
}
}
}
```
### See Also
* enum [PdfCustomPropertiesExport](../../../aspose.cells.rendering/pdfcustompropertiesexport/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
