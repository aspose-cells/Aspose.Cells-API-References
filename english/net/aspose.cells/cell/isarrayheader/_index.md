---
title: Cell.IsArrayHeader
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates the cells formula is an array formula and it is the first cell of the array
type: docs
url: /net/aspose.cells/cell/isarrayheader/
---
## Cell.IsArrayHeader property

Indicates the cell's formula is an array formula and it is the first cell of the array.

```csharp
public bool IsArrayHeader { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(cell.IsArrayHeader, &amp;quot;A1(Single-True).IsArrayHeader&amp;quot;); //CELLSNET-43695
[Test]
        public void Property_IsArrayHeader()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            //cells.MemorySetting = MemorySetting.MemoryPreference;
            Cell cell = cells[&quot;A1&quot;];
            cell.SetArrayFormula(&quot;=B1:D1&quot;, 1, 1);
            cells[&quot;B1&quot;].PutValue(&quot;#VALUE!&quot;);
            wb.CalculateFormula();
            cell.RemoveArrayFormula(false);
            Assert.IsFalse(cell.IsFormula, &quot;A1(Single-False).IsFormula&quot;);
            Assert.AreEqual(&quot;#VALUE!&quot;, cell.Value, &quot;A1(Single-False).Value&quot;);

            cell.SetArrayFormula(&quot;=B1:D1&quot;, 1, 1);
            cell.RemoveArrayFormula(true);
            Assert.IsFalse(cell.IsArrayHeader, &quot;A1(Single-True).IsArrayHeader&quot;); //CELLSNET-43695
            Assert.IsFalse(cell.IsArrayFormula, &quot;A1(Single-True).IsArrayHeader&quot;);
            Assert.AreEqual(&quot;=B1:D1&quot;, cell.Formula, &quot;A1(Single-True).Formula&quot;);

            cell.SetArrayFormula(&quot;=B1:D1&quot;, 1, 3);
            cells[&quot;D1&quot;].PutValue(&quot;#VALUE!&quot;);
            wb.CalculateFormula();
            cell.RemoveArrayFormula(false);
            for (int i = 0; i &lt; 3; i++)
            {
                char cn = (char)(&apos;A&apos; + i);
                cell = cells[0, i];
                Assert.IsFalse(cell.IsFormula, cn + &quot;1(Multiple-False).IsFormula&quot;);
                Assert.AreEqual(&quot;#VALUE!&quot;, cell.Value, cn + &quot;1(Multiple-False).Value&quot;);
            }

            cell = cells[&quot;A1&quot;];
            cell.SetArrayFormula(&quot;=B1:D1&quot;, 1, 3);
            cell.RemoveArrayFormula(true);
            for (int i = 0; i &lt; 3; i++)
            {
                char cn = (char)(&apos;A&apos; + i);
                cell = cells[0, i];
                Assert.IsFalse(cell.IsArrayHeader, cn + &quot;1(Multiple-True).IsArrayHeader&quot;);
                Assert.IsFalse(cell.IsArrayFormula, cn + &quot;1(Multiple-True).IsInArray&quot;);
                Assert.AreEqual(&quot;=B1:D1&quot;, cell.Formula, cn + &quot;1(Multiple-True).Formula&quot;);
            }
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


