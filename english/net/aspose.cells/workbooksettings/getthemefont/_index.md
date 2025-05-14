---
title: WorkbookSettings.GetThemeFont
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings method. Gets the default theme font name
type: docs
url: /net/aspose.cells/workbooksettings/getthemefont/
---
## WorkbookSettings.GetThemeFont method

Gets the default theme font name.

```csharp
public string GetThemeFont(FontSchemeType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | FontSchemeType | The scheme type of the font. |

### Examples

```csharp
// Called: Assert.AreEqual("Calibri", w.Settings.GetThemeFont(FontSchemeType.Minor));
public void WorkbookSettings_Method_GetThemeFont()
{
    Workbook workbook = new Workbook();
    workbook.Protect(ProtectionType.Windows, "test");
    Assert.AreEqual(workbook.Settings.ProtectionType, ProtectionType.Windows);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(workbook.Settings.ProtectionType, ProtectionType.Windows);
    Workbook w = new Workbook();
    w.Settings.IsMinimized = true;
    w.Save(Constants.destPath + "IsMinimized.xlsx");
    w= new Workbook(Constants.destPath + "IsMinimized.xlsx");
    Assert.IsTrue(w.Settings.IsMinimized);
    Assert.AreEqual("Calibri", w.Settings.GetThemeFont(FontSchemeType.Minor));
    Assert.AreEqual("9302", w.Settings.BuildVersion);
}
```

### See Also

* enum [FontSchemeType](../../fontschemetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


