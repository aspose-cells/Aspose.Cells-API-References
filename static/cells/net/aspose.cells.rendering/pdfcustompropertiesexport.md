##Enum PdfCustomPropertiesExport
Aspose.Cells.Rendering.PdfCustomPropertiesExport enum. Specifies the way CustomDocumentPropertyCollection are exported to PDF file
## PdfCustomPropertiesExport enumeration
Specifies the way [`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection/) are exported to PDF file.
```csharp
public enum PdfCustomPropertiesExport
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No custom properties are exported. |
| Standard | `1` | Custom properties are exported as entries in Info dictionary. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class PdfCustomPropertiesExportDemo
{
public static void PdfCustomPropertiesExportExample()
{
// Create a workbook and add some data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello Aspose");
worksheet.Cells["A2"].PutValue("This is a sample document");
// Set some custom properties
workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
workbook.Worksheets.CustomDocumentProperties.Add("Subject", "Sample PDF Export");
// Create PDF save options
PdfSaveOptions saveOptions = new PdfSaveOptions();
// Set the custom properties export option
saveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;
// Save the workbook to PDF
workbook.Save("PdfCustomPropertiesExportExample.pdf", saveOptions);
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
