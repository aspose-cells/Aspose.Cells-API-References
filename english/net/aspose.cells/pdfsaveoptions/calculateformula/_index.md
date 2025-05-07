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
// Called: options.CalculateFormula = true;
[Test]
        public void Property_CalculateFormula()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "SAASCELLS-157-1.xltx");
            PdfSaveOptions options = new PdfSaveOptions();
            options.CalculateFormula = true;
            options.SetImageResample(90, 70);

            workbook.Save(new MemoryStream(), options);
        }
```

### See Also

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


