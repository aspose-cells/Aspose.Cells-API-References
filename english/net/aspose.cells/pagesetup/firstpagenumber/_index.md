---
title: PageSetup.FirstPageNumber
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the first page number that will be used when this sheet is printed
type: docs
url: /net/aspose.cells/pagesetup/firstpagenumber/
---
## PageSetup.FirstPageNumber property

Represents the first page number that will be used when this sheet is printed.

```csharp
public int FirstPageNumber { get; set; }
```

### Examples

```csharp
// Called: worksheet.PageSetup.FirstPageNumber = 1;
[Test]
        public void Property_FirstPageNumber()
        {
            Workbook document = new Workbook(Constants.sourcePath + "CELLSNET56098.xlsx");
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

            document.Save(Constants.destPath + "CELLSNET56098.pdf", pdfSaveOptions);//exception
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


