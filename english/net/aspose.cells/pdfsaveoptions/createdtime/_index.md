---
title: PdfSaveOptions.CreatedTime
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions property. Gets and sets the time of generating the pdf document
type: docs
url: /net/aspose.cells/pdfsaveoptions/createdtime/
---
## PdfSaveOptions.CreatedTime property

Gets and sets the time of generating the pdf document.

```csharp
public DateTime CreatedTime { get; set; }
```

### Remarks

if it is not be set, it will be the time of generating the pdf.

### Examples

```csharp
// Called: CreatedTime = DateTime.Now,
public void PdfSaveOptions_Property_CreatedTime()
{
    Workbook wb = new Workbook();
    wb.Worksheets[0].Cells["A1"].Value = "PdfA/1b validation with CreateTime setting";

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
            Assert.IsTrue(content.IndexOf("/ID") != -1);
        }
    }
}
```

### See Also

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


