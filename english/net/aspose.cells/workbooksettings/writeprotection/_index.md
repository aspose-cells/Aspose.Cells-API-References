---
title: WorkbookSettings.WriteProtection
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Provides access to the workbook write protection options
type: docs
url: /net/aspose.cells/workbooksettings/writeprotection/
---
## WorkbookSettings.WriteProtection property

Provides access to the workbook write protection options.

```csharp
public WriteProtection WriteProtection { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("abc", workbook.Settings.WriteProtection.Author);
public void WorkbookSettings_Property_WriteProtection()
{

    Workbook workbook = new Workbook();

    workbook.Settings.WriteProtection.Password = "test";
    workbook.Settings.WriteProtection.Author = "abc";
    workbook.Save(Constants.destPath + "WriteProtection1.xlsx");
    workbook = new Workbook(Constants.destPath + "WriteProtection1.xlsx");
    Assert.AreEqual("abc", workbook.Settings.WriteProtection.Author);

}
```

### See Also

* class [WriteProtection](../../writeprotection/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


