---
title: Cells.Count
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the total count of instantiated Cell objects
type: docs
url: /net/aspose.cells/cells/count/
---
## Cells.Count property

Gets the total count of instantiated Cell objects.

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(350, cells.Count, "CellCount");
[Test]
        public void Property_Count()
        {
            Workbook wb = new Workbook();
            Style ds = wb.DefaultStyle;
            ds.Custom = "00000";
            Cells cells = wb.Worksheets[0].Cells;
            bool odd = false;
            for (int i = 0; i < 70; i++)
            {
                for (int j = odd ? 1 : 0; j < 10; j += 2)
                {
                    cells[i, j].PutValue(i * 10 + j);
                }
                odd = !odd;
            }
            cells.RemoveDuplicates(); //IndexOutOfRangeException
            Assert.AreEqual(69, cells.MaxDataRow, "MaxDataRow");
            Assert.AreEqual(350, cells.Count, "CellCount");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


