---
title: LoadOptions.MemorySetting
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets or sets the memory usage options
type: docs
url: /net/aspose.cells/loadoptions/memorysetting/
---
## LoadOptions.MemorySetting property

Gets or sets the memory usage options.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Examples

```csharp
// Called: op.MemorySetting = MemorySetting.MemoryPreference;
[Test]
        public void Property_MemorySetting()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSNET52299.xlsx");
            Assert.IsTrue(wb.HasRevisions);
            LoadOptions op = new LoadOptions();
            op.MemorySetting = MemorySetting.MemoryPreference;
            wb = new Workbook(Constants.sourcePath + "CELLSNET52299.xlsx", op);
            wb = Util.ReSave(wb, SaveFormat.Xlsx);
            Assert.IsTrue(wb.HasRevisions);
        }
```

### See Also

* enum [MemorySetting](../../memorysetting/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


