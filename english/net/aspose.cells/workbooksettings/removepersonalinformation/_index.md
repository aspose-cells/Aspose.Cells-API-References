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
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet42312.xlsx&quot;);
            Assert.AreEqual(workbook.Settings.RemovePersonalInformation, true);
            workbook.Save(Constants.destPath + &quot;CellsNet42312.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet42312.xlsx&quot;);
            Assert.AreEqual(workbook.Settings.RemovePersonalInformation, true);
            workbook.Save(Constants.destPath + &quot;CellsNet42312.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet42312.xls&quot;);
            Assert.AreEqual(workbook.Settings.RemovePersonalInformation, true);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


