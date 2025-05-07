---
title: Workbook.Settings
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Represents the workbook settings
type: docs
url: /net/aspose.cells/workbook/settings/
---
## Workbook.Settings property

Represents the workbook settings.

```csharp
public WorkbookSettings Settings { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Settings.FirstVisibleTab, 1);
[Test]
        public void Property_Settings()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava40957.xlsx");
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            Assert.AreEqual(workbook.Settings.FirstVisibleTab, 1);
        }
```

### See Also

* class [WorkbookSettings](../../workbooksettings/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


