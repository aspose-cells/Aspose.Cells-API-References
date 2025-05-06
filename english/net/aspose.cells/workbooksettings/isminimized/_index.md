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
// Called: Assert.IsTrue(w.Settings.IsMinimized);
[Test]
        public void Property_IsMinimized()
        {
            Workbook workbook = new Workbook();
            workbook.Protect(ProtectionType.Windows, &quot;test&quot;);
            Assert.AreEqual(workbook.Settings.ProtectionType, ProtectionType.Windows);
            workbook.Save(Constants.destPath + &quot;Protect01.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;Protect01.xlsx&quot;);
            Assert.AreEqual(workbook.Settings.ProtectionType, ProtectionType.Windows);
            Workbook w = new Workbook();
            w.Settings.IsMinimized = true;
            w.Save(Constants.destPath + &quot;IsMinimized.xlsx&quot;);
            w= new Workbook(Constants.destPath + &quot;IsMinimized.xlsx&quot;);
            Assert.IsTrue(w.Settings.IsMinimized);
            Assert.AreEqual(&quot;Calibri&quot;, w.Settings.GetThemeFont(FontSchemeType.Minor));
            Assert.AreEqual(&quot;9302&quot;, w.Settings.BuildVersion);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


