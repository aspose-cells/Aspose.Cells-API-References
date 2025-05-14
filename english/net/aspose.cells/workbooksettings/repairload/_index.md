---
title: WorkbookSettings.RepairLoad
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Indicates whether the application last opened the workbook in safe or repair mode
type: docs
url: /net/aspose.cells/workbooksettings/repairload/
---
## WorkbookSettings.RepairLoad property

Indicates whether the application last opened the workbook in safe or repair mode.

```csharp
public bool RepairLoad { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.RepairLoad = true;
public void WorkbookSettings_Property_RepairLoad()
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


