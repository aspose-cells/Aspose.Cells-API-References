---
title: Cells.AddRange
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Adds a range object reference to cells
type: docs
url: /net/aspose.cells/cells/addrange/
---
## Cells.AddRange method

Adds a range object reference to cells

```csharp
public void AddRange(Range rangeObject)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rangeObject | Range | The range object will be contained in the cells |

### Examples

```csharp
// Called: cells.AddRange(range);
[Test]
        public void Method_Range_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange(&quot;A1&quot;, &quot;B2&quot;);
            cells.AddRange(range);
            range.Name = &quot;TestNamedRange&quot;;
            cells.InsertColumn(1);
            cells.InsertRow(1);
            Assert.AreEqual(range.RowCount, 3);
            Assert.AreEqual(range.ColumnCount, 3);
            cells.InsertColumns(1, 4);
            Assert.AreEqual(range.ColumnCount, 7);
        }
```

### See Also

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


