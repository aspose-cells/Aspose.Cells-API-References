---
title: PdfSaveOptions.CustomPropertiesExport
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions property. Gets or sets a value determining the way CustomDocumentPropertyCollection are exported to PDF file. Default value is None
type: docs
url: /net/aspose.cells/pdfsaveoptions/custompropertiesexport/
---
## PdfSaveOptions.CustomPropertiesExport property

Gets or sets a value determining the way [`CustomDocumentPropertyCollection`](../../../aspose.cells.properties/customdocumentpropertycollection/) are exported to PDF file. Default value is None.

```csharp
public PdfCustomPropertiesExport CustomPropertiesExport { get; set; }
```

### Examples

```csharp
// Called: saveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;
public static void PdfSaveOptions_Property_CustomPropertiesExport()
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
```

### See Also

* enum [PdfCustomPropertiesExport](../../../aspose.cells.rendering/pdfcustompropertiesexport/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


