---
title: WorkbookSettings.ProtectionType
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets the protection type of the workbook
type: docs
url: /net/aspose.cells/workbooksettings/protectiontype/
---
## WorkbookSettings.ProtectionType property

Gets the protection type of the workbook.

```csharp
public ProtectionType ProtectionType { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Settings.ProtectionType, ProtectionType.Windows);
public void WorkbookSettings_Property_ProtectionType()
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

* enum [ProtectionType](../../protectiontype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


