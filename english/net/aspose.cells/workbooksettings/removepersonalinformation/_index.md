---
title: WorkbookSettings.RemovePersonalInformation
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. True if personal information can be removed from the specified workbook
type: docs
url: /net/aspose.cells/workbooksettings/removepersonalinformation/
---
## WorkbookSettings.RemovePersonalInformation property

True if personal information can be removed from the specified workbook.

```csharp
public bool RemovePersonalInformation { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Settings.RemovePersonalInformation, true);
[Test]
        public void Property_RemovePersonalInformation()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet42312.xlsx");
            Assert.AreEqual(workbook.Settings.RemovePersonalInformation, true);
            workbook.Save(Constants.destPath + "CellsNet42312.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet42312.xlsx");
            Assert.AreEqual(workbook.Settings.RemovePersonalInformation, true);
            workbook.Save(Constants.destPath + "CellsNet42312.xls");
            workbook = new Workbook(Constants.destPath + "CellsNet42312.xls");
            Assert.AreEqual(workbook.Settings.RemovePersonalInformation, true);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


