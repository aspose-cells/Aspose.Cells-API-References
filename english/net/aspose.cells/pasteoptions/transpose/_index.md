---
title: PasteOptions.Transpose
second_title: Aspose.Cells for .NET API Reference
description: PasteOptions property. True to transpose rows and columns when the range is pasted. The default value is False
type: docs
url: /net/aspose.cells/pasteoptions/transpose/
---
## PasteOptions.Transpose property

True to transpose rows and columns when the range is pasted. The default value is False.

```csharp
public bool Transpose { get; set; }
```

### Examples

```csharp
// Called: opt.Transpose = true;
[Ignore("Not supported yet")]
        public void Property_Transpose()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].PutValue(1);
            cells[1, 0].PutValue(2);
            cells[2, 0].Formula = "=A1+A2";
            wb.CalculateFormula(false);

            Aspose.Cells.Range src = cells.CreateRange("A1:A3");
            Aspose.Cells.Range dest = cells.CreateRange("B1:D1");

            PasteOptions opt = new PasteOptions();
            opt.PasteType = PasteType.All;
            opt.Transpose = true;
            dest.Copy(src, opt);
            Assert.AreEqual("=B1+C1", cells[0, 3].Formula, "TransposeCopied formula");
        }
```

### See Also

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


