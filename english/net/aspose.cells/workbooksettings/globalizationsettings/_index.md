---
title: WorkbookSettings.GlobalizationSettings
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets and sets the globalization settings
type: docs
url: /net/aspose.cells/workbooksettings/globalizationsettings/
---
## WorkbookSettings.GlobalizationSettings property

Gets and sets the globalization settings.

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

### Examples

```csharp
// Called: wb.Settings.GlobalizationSettings = new MG();
[Test]
        public void Property_GlobalizationSettings()
        {
            Workbook wb = new Workbook();
            wb.Settings.GlobalizationSettings = new MG();
           Assert.AreEqual(&quot;Tabellenblatt2&quot;,wb.Worksheets[wb.Worksheets.Add()].Name);
        }
```

### See Also

* class [GlobalizationSettings](../../globalizationsettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


