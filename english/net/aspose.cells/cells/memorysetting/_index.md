---
title: Cells.MemorySetting
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets or sets the memory usage option for this cells
type: docs
url: /net/aspose.cells/cells/memorysetting/
---
## Cells.MemorySetting property

Gets or sets the memory usage option for this cells.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Examples

```csharp
// Called: cells.MemorySetting = MemorySetting.MemoryPreference;
[Test]
        public void Property_MemorySetting()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells.MemorySetting = MemorySetting.MemoryPreference;
            for (int i = 0; i < 80; i++)
            {
                double dv = cells.Rows[i].Height;
            }
            cells[0, 0].PutValue(1);
            cells[1, 0].PutValue(2);
            cells.DeleteRows(0, 1);
            Assert.AreEqual(2, cells[0, 0].IntValue, "After delete, A1's value");
        }
```

### See Also

* enum [MemorySetting](../../memorysetting/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


