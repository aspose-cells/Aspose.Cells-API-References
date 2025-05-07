---
title: Name.SheetIndex
second_title: Aspose.Cells for .NET API Reference
description: Name property. Indicates this name belongs to Workbook or Worksheet. 0  Global name otherwise index to sheet onebased
type: docs
url: /net/aspose.cells/name/sheetindex/
---
## Name.SheetIndex property

Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based)

```csharp
public int SheetIndex { get; set; }
```

### Examples

```csharp
// Called: + (name.SheetIndex == 0 ? ": GLOBAL" : ": LOCAL")
[Test]
        public void Property_SheetIndex()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "J42118_815971.xlsx");
            NameCollection names = wb.Worksheets.Names;
            StringBuilder sb = new StringBuilder();
            for (int i = names.Count - 1; i > -1; i--)
            {
                Name name = names[i];

                // determine the Refers To Type (reference|formula)
                Aspose.Cells.Range[] rs = name.GetRanges();
                if (rs != null && rs.Length > 0 && rs[0] == null)
                {
                    // ERROR: name.getRanges().length is > 0 - BUT name.getRanges()[0] is null
                    sb.Append("\nERROR! Invalid Name.GetRanges() for " + name.FullText
                              + (name.SheetIndex == 0 ? ": GLOBAL" : ": LOCAL")
                              + ", Visible=" + name.IsVisible + ", RefersTo=" + name.RefersTo);
                }
            }
            if (sb.Length > 0)
            {
                Assert.Fail(sb.ToString());
            }
            Cell cell = wb.Worksheets[0].Cells[10, 0];
            cell.Formula = "=_HC1";
            wb.CalculateFormula(false);
            Assert.AreEqual("#NAME?", cell.Value, "SelfReference Name's calculated result");
        }
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


