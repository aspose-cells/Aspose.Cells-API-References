---
title: WorkbookSettings.IsHidden
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Indicates whether this workbook is hidden
type: docs
url: /net/aspose.cells/workbooksettings/ishidden/
---
## WorkbookSettings.IsHidden property

Indicates whether this workbook is hidden.

```csharp
public bool IsHidden { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(workbook.Settings.IsHidden);
[Test]
        public void Property_IsHidden()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET45757.xls");
            Assert.IsFalse(workbook.Settings.IsHidden);
            workbook.Save(Constants.destPath + "CELLSNET45757.xls");
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


