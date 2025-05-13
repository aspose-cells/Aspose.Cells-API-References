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
// Called: Compliance = Aspose.Cells.Rendering.PdfCompliance.PdfA1b
public void PdfSaveOptions_Property_Compliance()
{
    string filePath = Constants.PivotTableSourcePath + @"NET46510_";
    var workbook = new Workbook(filePath + "example.xlsx");
    var options = new Aspose.Cells.PdfSaveOptions
    {
        Compliance = Aspose.Cells.Rendering.PdfCompliance.PdfA1b
    };
    workbook.Save(CreateFolder(filePath) + "out.pdf", options);
}
```

### See Also

* enum [PdfCompliance](../../../aspose.cells.rendering/pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


