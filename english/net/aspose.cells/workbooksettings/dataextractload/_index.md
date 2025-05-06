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
// Called: Assert.AreEqual(workbook.Settings.DataExtractLoad, true);
[Test]
        public void Property_DataExtractLoad()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.AutoRecover = false;
            workbook.Settings.DataExtractLoad = true;
            workbook.Settings.CrashSave = true;
            workbook.Settings.RepairLoad = true;
            workbook.Save(Constants.destPath +&quot;CellsNet43158.xlsx&quot;);
            workbook = new Workbook(Constants.destPath +&quot;CellsNet43158.xlsx&quot;);
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


