---
title: AutoFilter.Filter
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Filters a list with specified criteria
type: docs
url: /net/aspose.cells/autofilter/filter/
---
## AutoFilter.Filter method

Filters a list with specified criteria.

```csharp
public void Filter(int fieldIndex, string criteria)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | String | The specified criteria (a string; for example, "101"). |

### Remarks

Aspose.Cells will remove all other filter setting on this field as Ms Excel 97-2003.

### Examples

```csharp
// Called: sheet.AutoFilter.Filter(1, "Nom2");
public void AutoFilter_Method_Filter()
{
    Aspose.Cells.License license = new Aspose.Cells.License();
    license.SetLicense(Constants.licPath);
    Workbook workbook = new Workbook(Constants.sourcePath + "AutoFilter/aa_filtre.xls");
    Worksheet sheet = workbook.Worksheets[0];
    sheet.AutoFilter.SetRange(0, 0, 1);
    sheet.AutoFilter.Filter(1, "Nom2");
    sheet.AutoFilter.Refresh();
    Assert.AreEqual(sheet.Cells.GetRowHeight(3), 0);

    Assert.AreEqual(sheet.Cells.GetRowHeight(4), 0);
    Util.ReSave(workbook, SaveFormat.Excel97To2003);//.Save(Constants.destPath + "aa_filtre.xls");
}
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


