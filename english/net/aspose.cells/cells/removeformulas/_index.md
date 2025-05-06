---
title: Cells.RemoveFormulas
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Removes all formula and replaces with the value of the formula
type: docs
url: /net/aspose.cells/cells/removeformulas/
---
## Cells.RemoveFormulas method

Removes all formula and replaces with the value of the formula.

```csharp
public void RemoveFormulas()
```

### Examples

```csharp
// Called: cells.RemoveFormulas();
[Test]
        public void Method_RemoveFormulas()
        {
            Workbook wb = new Workbook(FileFormatType.Xlsx);
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].SetSharedFormula(&quot;=IF(TRUE,\&quot;\&quot;,1)&quot;, 5, 1);
            cells[0, 2].PutValue(1);
            cells[1, 2].PutValue(1);
            cells[3, 2].PutValue(1);
            for (int i = 0; i &lt; 5; i++)
            {
                cells.Merge(i, 0, 1, 2);
            }
            wb.CalculateFormula();
            Assert.AreEqual(5, cells.Rows.Count);
            int count = 0;
            IEnumerator en = cells.Rows.GetEnumerator();
            while (en.MoveNext())
            {
                Row r = (Row)en.Current;
                Assert.IsFalse(r.IsBlank, &quot;IsBlank for row index &quot; + r.Index);
                count++;
            }
            Assert.AreEqual(5, count);
            cells.DeleteBlankRows();
            Assert.AreEqual(5, cells.Rows.Count);
            cells.RemoveFormulas();
            Assert.AreEqual(5, cells.Rows.Count);
            en = cells.Rows.GetEnumerator();
            count = 0;
            while (en.MoveNext())
            {
                Row r = (Row)en.Current;
                if (r.Index == 2 || r.Index == 4)
                {
                    Assert.IsTrue(r.IsBlank, &quot;IsBlank for row index &quot; + r.Index);
                }
                else
                {
                    Assert.IsFalse(r.IsBlank, &quot;IsBlank for row index &quot; + r.Index);
                }
                count++;
            }
            Assert.AreEqual(5, count);
            cells.DeleteBlankRows();
            Assert.AreEqual(3, cells.Rows.Count);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


