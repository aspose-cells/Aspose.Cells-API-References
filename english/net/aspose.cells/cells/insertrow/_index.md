---
title: Cells.InsertRow
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Inserts a new row into the worksheet
type: docs
url: /net/aspose.cells/cells/insertrow/
---
## Cells.InsertRow method

Inserts a new row into the worksheet.

```csharp
public void InsertRow(int rowIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |

### Examples

```csharp
// Called: cells.InsertRow(32);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells.MemorySetting = MemorySetting.MemoryPreference;
            for (int i = 0; i &lt; 120; i++)
            {
                cells[i, 0].PutValue(i);
            }
            cells.InsertRow(32);
            for (int i = 0; i &lt; 32; i++)
            {
                Assert.AreEqual(i, cells[i, 0].IntValue, &quot;After insert, row &quot; + i);
            }
            for (int i = 33; i &lt; 120; i++)
            {
                Assert.AreEqual(i - 1, cells[i, 0].IntValue, &quot;After insert, row &quot; + i);
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


