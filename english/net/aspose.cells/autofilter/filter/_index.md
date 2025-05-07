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
// Called: sheet.AutoFilter.Filter(2, "Pending");
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "AutoFilter/aa_filtre_002.xls");
            Worksheet sheet = workbook.Worksheets[0];
            sheet.AutoFilter.SetRange(0, 0, 2);
            sheet.AutoFilter.Filter(2, "Pending");
            sheet.AutoFilter.Refresh();
            Assert.AreEqual(sheet.Cells.GetRowHeight(1), 0);

            Assert.AreEqual(sheet.Cells.GetRowHeight(2), 0);
            workbook.Save(Constants.destPath + "aa_filtre_002.xls");
        }
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


