---
title: PageSetup.Orientation
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents page print orientation
type: docs
url: /net/aspose.cells/pagesetup/orientation/
---
## PageSetup.Orientation property

Represents page print orientation.

```csharp
public PageOrientationType Orientation { get; set; }
```

### Examples

```csharp
// Called: worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
public void PageSetup_Property_Orientation()
{
    Workbook document = new Workbook(Constants.sourcePath + "example.xlsx");
    document.BuiltInDocumentProperties.Title = "defaultTitle";
    document.BuiltInDocumentProperties.Author = "defaultAuthor";
    document.BuiltInDocumentProperties.Subject = "defaultSubject";

    foreach (Worksheet worksheet in document.Worksheets)
    {
        worksheet.PageSetup.PaperSize = PaperSizeType.PaperA4;
        worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
        worksheet.PageSetup.FirstPageNumber = 1;
        worksheet.PageSetup.Zoom = 100;
    }

    var pdfSaveOptions = new PdfSaveOptions();
    pdfSaveOptions.Compliance = PdfCompliance.PdfA1b;

    document.Save(Constants.destPath + "example.pdf", pdfSaveOptions);//exception
}
```

### See Also

* enum [PageOrientationType](../../pageorientationtype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


