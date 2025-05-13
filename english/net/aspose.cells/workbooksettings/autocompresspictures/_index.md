---
title: WorkbookSettings.AutoCompressPictures
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Specifies a boolean value that indicates the application automatically compressed pictures in the workbook
type: docs
url: /net/aspose.cells/workbooksettings/autocompresspictures/
---
## WorkbookSettings.AutoCompressPictures property

Specifies a boolean value that indicates the application automatically compressed pictures in the workbook.

```csharp
public bool AutoCompressPictures { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Settings.AutoCompressPictures);
public void WorkbookSettings_Property_AutoCompressPictures()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.IsTrue(workbook.Settings.AutoCompressPictures);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.IsTrue(workbook.Settings.AutoCompressPictures);
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


