---
title: Cell.IsArrayFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates whether the cell formula is an array formula
type: docs
url: /net/aspose.cells/cell/isarrayformula/
---
## Cell.IsArrayFormula property

Indicates whether the cell formula is an array formula.

```csharp
public bool IsArrayFormula { get; }
```

### Examples

```csharp
// Called: if (!cells[i, 0].IsArrayFormula)
[Test]
        public void Property_IsArrayFormula()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].SetArrayFormula(&quot;=B1:B3&quot;, 3, 1);
            for (int i = 0; i &lt; 3; i++)
            {
                if (!cells[i, 0].IsArrayFormula)
                {
                    Assert.Fail(&quot;A&quot; + (i + 1) + &quot; should be set as array formula&quot;);
                }
            }
            wb = Util.ReSave(wb, SaveFormat.Xlsb);
            cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 3; i++)
            {
                if (!cells[i, 0].IsArrayFormula)
                {
                    Assert.Fail(&quot;A&quot; + (i + 1) + &quot; should be read as array formula&quot;);
                }
            }
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


