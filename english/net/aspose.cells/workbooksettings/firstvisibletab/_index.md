---
title: WorkbookSettings.FirstVisibleTab
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets or sets the first visible worksheet tab
type: docs
url: /net/aspose.cells/workbooksettings/firstvisibletab/
---
## WorkbookSettings.FirstVisibleTab property

Gets or sets the first visible worksheet tab.

```csharp
public int FirstVisibleTab { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Settings.FirstVisibleTab, 1);
public void WorkbookSettings_Property_FirstVisibleTab()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    Assert.AreEqual(workbook.Settings.FirstVisibleTab, 1);
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


