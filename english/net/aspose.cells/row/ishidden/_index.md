---
title: Row.IsHidden
second_title: Aspose.Cells for .NET API Reference
description: Row property. Indicates whether the row is hidden
type: docs
url: /net/aspose.cells/row/ishidden/
---
## Row.IsHidden property

Indicates whether the row is hidden.

```csharp
public bool IsHidden { get; set; }
```

### Examples

```csharp
// Called: cells.Rows[1].IsHidden = true;
public void Property_IsHidden()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 6; i++)
            {
                cells[i, 0].PutValue(6 - i);
            }
            cells.Rows[1].IsHidden = true;
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);
            sorter.Sort(cells, 0, 0, 5, 0);
            Assert.AreEqual(1, cells[0, 0].IntValue, &quot;A1&quot;);
            Assert.AreEqual(5, cells[1, 0].IntValue, &quot;A2&quot;);
            Assert.IsTrue(cells.Rows[1].IsHidden, &quot;The second row should be hidden and should not be sorted&quot;);
            Assert.AreEqual(2, cells[2, 0].IntValue, &quot;A3&quot;);
            Assert.AreEqual(3, cells[3, 0].IntValue, &quot;A4&quot;);
            Assert.AreEqual(4, cells[4, 0].IntValue, &quot;A5&quot;);
            Assert.AreEqual(6, cells[5, 0].IntValue, &quot;A6&quot;);
        }
```

### See Also

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


