---
title: PdfSaveOptions.CalculateFormula
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions property. Indicates whether to calculate formulas before saving pdf file
type: docs
url: /net/aspose.cells/pdfsaveoptions/calculateformula/
---
## PdfSaveOptions.CalculateFormula property

Indicates whether to calculate formulas before saving pdf file.

```csharp
public bool CalculateFormula { get; set; }
```

### Remarks

The default value is false.

### Examples

```csharp
// Called: pdfSaveOptions.CalculateFormula = true;
[Test]
        public void Property_CalculateFormula()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-55783.xlsx&quot;);

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.CalculateFormula = true;

            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, pdfSaveOptions);

                ms.Position = 0;
                using (StreamReader sr = new StreamReader(ms))
                {
                    string content = sr.ReadToEnd();
                    Assert.IsTrue(content.IndexOf(&quot;/Annot&quot;) != -1);
                }
            }
        }
```

### See Also

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


