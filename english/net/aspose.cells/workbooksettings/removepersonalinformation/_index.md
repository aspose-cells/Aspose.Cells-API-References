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
public void WorkbookSettings_Property_RemovePersonalInformation()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual(workbook.Settings.RemovePersonalInformation, true);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(workbook.Settings.RemovePersonalInformation, true);
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    Assert.AreEqual(workbook.Settings.RemovePersonalInformation, true);
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


