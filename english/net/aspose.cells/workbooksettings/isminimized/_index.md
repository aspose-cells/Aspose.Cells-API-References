---
title: WorkbookSettings.IsMinimized
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Represents whether the generated spreadsheet will be opened Minimized
type: docs
url: /net/aspose.cells/workbooksettings/isminimized/
---
## WorkbookSettings.IsMinimized property

Represents whether the generated spreadsheet will be opened Minimized.

```csharp
public bool IsMinimized { get; set; }
```

### Examples

```csharp
// Called: w.Settings.IsMinimized = true;
[Test]
        public void Property_IsMinimized()
        {
            Workbook workbook = new Workbook();
            workbook.Protect(ProtectionType.Windows, "test");
            Assert.AreEqual(workbook.Settings.ProtectionType, ProtectionType.Windows);
            workbook.Save(Constants.destPath + "Protect01.xlsx");
            workbook = new Workbook(Constants.destPath + "Protect01.xlsx");
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

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


