---
title: WorkbookSettings.MemorySetting
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets
type: docs
url: /net/aspose.cells/workbooksettings/memorysetting/
---
## WorkbookSettings.MemorySetting property

Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Examples

```csharp
// Called: wb.Settings.MemorySetting = MemorySetting.MemoryPreference;
public void WorkbookSettings_Property_MemorySetting()
{
    LoadOptions opts = new LoadOptions(LoadFormat.Xlsx);
    opts.MemorySetting = MemorySetting.MemoryPreference;
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx", opts);
    wb.Settings.MemorySetting = MemorySetting.MemoryPreference;
    wb.Save(new MemoryStream(), SaveFormat.Pdf);
}
```

### See Also

* enum [MemorySetting](../../memorysetting/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


