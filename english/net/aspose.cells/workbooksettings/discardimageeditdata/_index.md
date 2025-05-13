---
title: WorkbookSettings.DiscardImageEditData
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Indicates whether discarding editting image data
type: docs
url: /net/aspose.cells/workbooksettings/discardimageeditdata/
---
## WorkbookSettings.DiscardImageEditData property

Indicates whether discarding editting image data.

```csharp
public bool DiscardImageEditData { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(w.Settings.DiscardImageEditData);
public void WorkbookSettings_Property_DiscardImageEditData()
{
    Workbook w = new Workbook(Constants.sourcePath + @"example.xlsx");
    w.Save(Constants.destPath + "example.xlsb");
    w = new Workbook(Constants.destPath + "example.xlsb");
    w.Save(Constants.destPath + "example.xlsx");
    w = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(32767, w.Settings.DefaultImageResolution);
    Assert.IsFalse(w.Settings.DiscardImageEditData);
          

}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


