---
title: PdfSaveOptions.Compliance
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions property. Gets or sets the PDF standards compliance level for output documents
type: docs
url: /net/aspose.cells/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Gets or sets the PDF standards compliance level for output documents.

```csharp
public PdfCompliance Compliance { get; set; }
```

### Remarks

Default is Pdf17.

### Examples

```csharp
// Called: Compliance = PdfCompliance.PdfA1b
[Test]
        public void Property_Compliance()
        {
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells[&quot;A1&quot;].Value = &quot;PdfA/1b validation with CreateTime setting&quot;;

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions()
            {
                CreatedTime = DateTime.Now,
                Compliance = PdfCompliance.PdfA1b
            };

            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, pdfSaveOptions);

                ms.Position = 0;
                using (StreamReader sr = new StreamReader(ms))
                {
                    string content = sr.ReadToEnd();
                    Assert.IsTrue(content.IndexOf(&quot;/ID&quot;) != -1);
                }
            }
        }
```

### See Also

* enum [PdfCompliance](../../../aspose.cells.rendering/pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


