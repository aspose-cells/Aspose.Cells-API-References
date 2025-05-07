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
// Called: pdfSaveOptions.Compliance = pdfCompliance;
[Test]
        [Category("Checked")]
        public void Property_Compliance()
        {
            string FileName = Constants.sourcePath + "TestWorkbook\\Book2.xls";
            Workbook workbook = new Workbook(FileName);
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfCompliance pdfCompliance = PdfCompliance.None;
            pdfSaveOptions.Compliance = pdfCompliance;
            workbook.Save(Constants.checkPath + "PdfSaveOptions_Compliance_None.pdf", pdfSaveOptions);
        }
```

### See Also

* enum [PdfCompliance](../../../aspose.cells.rendering/pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


