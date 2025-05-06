---
title: FormulaParseOptions.R1C1Style
second_title: Aspose.Cells for .NET API Reference
description: FormulaParseOptions property. Whether the formula is R1C1 reference style. Default is false
type: docs
url: /net/aspose.cells/formulaparseoptions/r1c1style/
---
## FormulaParseOptions.R1C1Style property

Whether the formula is R1C1 reference style. Default is false.

```csharp
public bool R1C1Style { get; set; }
```

### Examples

```csharp
// Called: new FormulaParseOptions() { R1C1Style = true });
[Test]
        public void Property_R1C1Style()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[7, 4].SetArrayFormula(&quot;=TREND(RC[-1]:R[2]C[-1],RC[-2]:R[2]C[-2])&quot;, 3, 1,
                new FormulaParseOptions() { R1C1Style = true });
            for (int i = 7; i &lt; 10; i++)
            {
                Assert.AreEqual(&quot;=TREND(RC[-1]:R[2]C[-1],RC[-2]:R[2]C[-2])&quot;, cells[i, 4].R1C1Formula,
                    &quot;A&quot; + (i + 1) + &quot;.R1C1Formula(in arrayformula of E8:E10)&quot;);
            }
        }
```

### See Also

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


