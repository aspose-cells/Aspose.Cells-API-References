---
title: Cell.IsDynamicArrayFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates whether the cells formula is dynamic array formulatrue or legacy array formulafalse
type: docs
url: /net/aspose.cells/cell/isdynamicarrayformula/
---
## Cell.IsDynamicArrayFormula property

Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false).

```csharp
public bool IsDynamicArrayFormula { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(wb.Worksheets[0].Cells[0, 0].IsDynamicArrayFormula, "Resaved dynamic array formula");
[Test]
        public void Property_IsDynamicArrayFormula()
        {
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells[0, 0].SetDynamicArrayFormula("=B1:B3", new FormulaParseOptions(), false);
            wb = Util.ReSave(wb, SaveFormat.Xlsx);
            Assert.IsTrue(wb.Worksheets[0].Cells[0, 0].IsDynamicArrayFormula, "Resaved dynamic array formula");
            Workbook wb1 = new Workbook();
            wb1.Copy(wb);
            Assert.IsTrue(wb1.Worksheets[0].Cells[0, 0].IsDynamicArrayFormula, "Copied dynamic array formula");
            Util.SetHintMessage(wb1.Worksheets[0].Cells[0, 1],
                "Ms excel should not show error and A1.Formula should be dynamic array formula");
            MemoryStream ms = Util.SaveAsBuffer(wb1, SaveFormat.Xlsx);
            ms.Seek(0, SeekOrigin.Begin);
            if (!ManualFileUtil.ManualCheckStringInZip(ms, "xl/metadata.xml",
                new string[] { "name=\"XLDAPR\"", " fDynamic=" }, true))
            {
                Assert.Fail("Cannot find dynamic array formula related meta data in xl/metadata.xml in the genrated xlsx file");
            }
            File.WriteAllBytes(Constants.checkPath + "Formula/J43457N48039.xlsx", ms.ToArray());
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


