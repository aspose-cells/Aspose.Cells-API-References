---
title: WorkbookSettings.NumberGroupSeparator
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region
type: docs
url: /net/aspose.cells/workbooksettings/numbergroupseparator/
---
## WorkbookSettings.NumberGroupSeparator property

Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region.

```csharp
public char NumberGroupSeparator { get; set; }
```

### Examples

```csharp
// Called: wb.Settings.NumberGroupSeparator = '.';
public void WorkbookSettings_Property_NumberGroupSeparator()
{
    Workbook wb = new Workbook();
    wb.Settings.Region = CountryCode.USA;
    wb.Settings.NumberDecimalSeparator = ',';
    wb.Settings.NumberGroupSeparator = '.';
    Style style = wb.CreateStyle();
    style.Custom = "#,##0.00";
    Cell cell = wb.Worksheets[0].Cells[0, 0];
    cell.PutValue(12345.6798);
    cell.SetStyle(style);
    Assert.AreEqual("12.345,68", cell.StringValue, "12345.6798");
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


