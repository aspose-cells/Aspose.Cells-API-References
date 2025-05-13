---
title: WorkbookSettings.Date1904
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets or sets a value which represents if the workbook uses the 1904 date system
type: docs
url: /net/aspose.cells/workbooksettings/date1904/
---
## WorkbookSettings.Date1904 property

Gets or sets a value which represents if the workbook uses the 1904 date system.

```csharp
public bool Date1904 { get; set; }
```

### Examples

```csharp
// Called: wb.Settings.Date1904 = true;
public void WorkbookSettings_Property_Date1904()
{
    Workbook wb = new Workbook();
    wb.Settings.Date1904 = true;
    Cell cell = wb.Worksheets[0].Cells[0, 0];
    Style style = cell.GetStyle();
    style.Custom = "h:mm";
    cell.SetStyle(style);
    cell.PutValue(-0.0736111111111112);
    Assert.AreEqual("-1:46", cell.DisplayStringValue, "Negative time for Date1904");
    style.Custom = "mm/dd/yyyy h:mm:ss";
    cell.SetStyle(style);
    cell.PutValue(-42389.47075706);
    Assert.AreEqual("-01/21/2020 11:17:53", cell.DisplayStringValue, "Negative datetime for Date1904");
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


