---
title: WorkbookSettings.Password
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Represents Workbook file encryption password
type: docs
url: /net/aspose.cells/workbooksettings/password/
---
## WorkbookSettings.Password property

Represents Workbook file encryption password.

```csharp
public string Password { get; set; }
```

### Examples

```csharp
// Called: wb.Settings.Password = "xixi";
public void WorkbookSettings_Property_Password()
{
    LoadOptions loadOptions = new LoadOptions();
    Workbook wb = new Workbook(Constants.sourcePath + "example.ods", loadOptions);
    Assert.AreEqual("test encrypt.", wb.Worksheets[0].Cells["C6"].Value);
    wb.Settings.Password = "xixi";

    wb.Save(Constants.destPath + "example.ods");

    loadOptions.Password = "xixi";
    wb = new Workbook(Constants.destPath + "example.ods", loadOptions);
    Assert.AreEqual("test encrypt.", wb.Worksheets[0].Cells["C6"].Value);
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


