---
title: PdfSaveOptions.Producer
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions property. Gets and sets producer of generated pdf document
type: docs
url: /net/aspose.cells/pdfsaveoptions/producer/
---
## PdfSaveOptions.Producer property

Gets and sets producer of generated pdf document.

```csharp
public string Producer { get; set; }
```

### Remarks

If the value is null, or a valid LICENSE is not set, string Aspose.Cells vVERSION will be used.

### Examples

```csharp
// Called: pdfSaveOptions.Producer = "";
public void PdfSaveOptions_Property_Producer()
{
    Workbook wb = new Workbook();

    wb.Worksheets[0].Cells["A1"].PutValue("test Remove Pdf Producer");

    PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
    pdfSaveOptions.Producer = "";

    using (MemoryStream ms = new MemoryStream())
    {
        wb.Save(ms, pdfSaveOptions);

        ms.Position = 0;
        using(StreamReader sr = new StreamReader(ms))
        {
            string content = sr.ReadToEnd();
            Assert.IsTrue(content.IndexOf("/Producer") == -1);
        }
    }
}
```

### See Also

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


