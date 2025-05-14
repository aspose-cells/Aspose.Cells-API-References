---
title: PdfSaveOptions.PdfSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions constructor. Creates the options for saving pdf file
type: docs
url: /net/aspose.cells/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Creates the options for saving pdf file.

```csharp
public PdfSaveOptions()
```

### Examples

```csharp
// Called: PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
[Category("Checked")]
public void PdfSaveOptions_Constructor()
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

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


