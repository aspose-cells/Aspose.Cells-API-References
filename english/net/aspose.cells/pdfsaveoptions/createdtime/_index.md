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
// Called: pdfSaveOptions.CreatedTime = dt;
[Test]
        public void Property_CreatedTime()
        {
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells[&quot;A1&quot;].Value = &quot;Binary same if createdTime is set, and PDF/A or PDF/UA and pdf security are not set.&quot;;

            DateTime dt = new DateTime(2023, 11, 22);
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.CreatedTime = dt;

            MemoryStream ms = new MemoryStream();
            wb.Save(ms, pdfSaveOptions);
            byte[] bytes1 = ms.ToArray();

            ms = new MemoryStream();
            wb.Save(ms, pdfSaveOptions);
            byte[] bytes2 = ms.ToArray();

            Assert.AreEqual(bytes1.Length, bytes2.Length);
            int length = bytes1.Length;
            bool isSame = true;
            for(int i = 0; i &lt; length; i++)
            {
                if (bytes1[i] != bytes2[i])
                { 
                    isSame = false; 
                    break; 
                }
            }

            Assert.IsTrue(isSame);
        }
```

### See Also

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


