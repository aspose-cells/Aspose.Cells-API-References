---
title: WorkbookSettings.SetPageOrientationType
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings method. Set the type of print orientation for the whole workbook
type: docs
url: /net/aspose.cells/workbooksettings/setpageorientationtype/
---
## WorkbookSettings.SetPageOrientationType method

Set the type of print orientation for the whole workbook.

```csharp
public void SetPageOrientationType(PageOrientationType pageOrientationType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageOrientationType | PageOrientationType | The page orientation type |

### Examples

```csharp
// Called: workbook.Settings.SetPageOrientationType(PageOrientationType.Portrait);
public void WorkbookSettings_Method_SetPageOrientationType()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets.Add();
    workbook.Worksheets.Add();
    workbook.Settings.SetPageOrientationType(PageOrientationType.Portrait);
    foreach(Worksheet sheet in workbook.Worksheets)
    {
        Assert.AreEqual(PageOrientationType.Portrait, sheet.PageSetup.Orientation);
    }

}
```

### See Also

* enum [PageOrientationType](../../pageorientationtype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


