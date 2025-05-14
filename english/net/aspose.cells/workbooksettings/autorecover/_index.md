---
title: WorkbookSettings.AutoRecover
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Indicates whether the file is marked for autorecovery
type: docs
url: /net/aspose.cells/workbooksettings/autorecover/
---
## WorkbookSettings.AutoRecover property

Indicates whether the file is marked for auto-recovery.

```csharp
public bool AutoRecover { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Settings.AutoRecover, false);
public void WorkbookSettings_Property_AutoRecover()
{
    Workbook workbook = new Workbook();
    workbook.Settings.AutoRecover = false;
    workbook.Settings.DataExtractLoad = true;
    workbook.Settings.CrashSave = true;
    workbook.Settings.RepairLoad = true;
    workbook.Save(Constants.destPath +"example.xlsx");
    workbook = new Workbook(Constants.destPath +"example.xlsx");
    Assert.AreEqual(workbook.Settings.AutoRecover, false);
    Assert.AreEqual(workbook.Settings.DataExtractLoad, true);
    Assert.AreEqual(workbook.Settings.CrashSave, true);
    Assert.AreEqual(workbook.Settings.RepairLoad, true);
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


