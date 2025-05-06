---
title: PdfSaveOptions.FontEncoding
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions property. Gets or sets embedded font encoding in pdf
type: docs
url: /net/aspose.cells/pdfsaveoptions/fontencoding/
---
## PdfSaveOptions.FontEncoding property

Gets or sets embedded font encoding in pdf.

```csharp
public PdfFontEncoding FontEncoding { get; set; }
```

### Remarks

Default value is Identity

### Examples

```csharp
// Called: pdfSaveOptions.FontEncoding = PdfFontEncoding.AnsiPrefer;
public static void Property_FontEncoding()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello, Aspose!&quot;);

            // Create PdfSaveOptions and set the FontEncoding property
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.AnsiPrefer;

            // Save the workbook as a PDF file
            workbook.Save(&quot;PdfFontEncodingExample.pdf&quot;, pdfSaveOptions);

            Console.WriteLine(&quot;PDF file created successfully with specified font encoding.&quot;);
        }
```

### See Also

* enum [PdfFontEncoding](../../../aspose.cells.rendering/pdffontencoding/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


