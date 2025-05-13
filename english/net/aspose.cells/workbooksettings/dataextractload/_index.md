---
title: WorkbookSettings.DataExtractLoad
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. indicates whether the application last opened the workbook for data recovery
type: docs
url: /net/aspose.cells/workbooksettings/dataextractload/
---
## WorkbookSettings.DataExtractLoad property

indicates whether the application last opened the workbook for data recovery.

```csharp
public bool DataExtractLoad { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.DataExtractLoad = true;
public void WorkbookSettings_Property_DataExtractLoad()
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


