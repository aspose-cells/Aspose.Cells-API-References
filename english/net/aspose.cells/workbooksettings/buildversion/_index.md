---
title: WorkbookSettings.BuildVersion
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Specifies the incremental public release of the application
type: docs
url: /net/aspose.cells/workbooksettings/buildversion/
---
## WorkbookSettings.BuildVersion property

Specifies the incremental public release of the application.

```csharp
public string BuildVersion { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;9302&amp;quot;, w.Settings.BuildVersion);
[Test]
        public void Property_BuildVersion()
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


