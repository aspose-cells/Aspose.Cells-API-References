---
title: WorkbookSettings.Shared
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets or sets a value that indicates whether the Workbook is shared
type: docs
url: /net/aspose.cells/workbooksettings/shared/
---
## WorkbookSettings.Shared property

Gets or sets a value that indicates whether the Workbook is shared.

```csharp
public bool Shared { get; set; }
```

### Remarks

The default value is false.

### Examples

```csharp
// Called: wb.Settings.Shared = true;
[Test]
        public void Property_Shared()
        {

            Workbook wb = new Workbook();

            wb.Settings.Shared = true;
            wb.Save(Constants.destPath + "CellsNet54387_shared.xlsx");

            wb.Settings.Shared = false;

            wb.Save(Constants.destPath + "Test1_notShared.xlsx");
            wb = new Workbook(Constants.destPath + "Test1_notShared.xlsx");
            Assert.IsFalse(wb.Settings.Shared);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


