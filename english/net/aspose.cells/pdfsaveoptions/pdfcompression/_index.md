---
title: PdfSaveOptions.PdfCompression
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions property. Indicate the compression algorithm
type: docs
url: /net/aspose.cells/pdfsaveoptions/pdfcompression/
---
## PdfSaveOptions.PdfCompression property

Indicate the compression algorithm

```csharp
public PdfCompressionCore PdfCompression { get; set; }
```

### Examples

```csharp
// Called: pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate; // Setting the compression type to Flate
public static void Property_PdfCompression()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello Aspose!&quot;);

            // Create PdfSaveOptions and set the PdfCompressionCore
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate; // Setting the compression type to Flate

            // Save the workbook as a PDF file with the specified compression
            workbook.Save(&quot;PdfCompressionCoreExample.pdf&quot;, pdfSaveOptions);

            Console.WriteLine(&quot;PDF file saved with specified compression.&quot;);
        }
```

### See Also

* enum [PdfCompressionCore](../../../aspose.cells.rendering/pdfcompressioncore/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


