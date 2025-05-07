---
title: AutoFilter.FilterTop10
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Filter the top 10 item in the list
type: docs
url: /net/aspose.cells/autofilter/filtertop10/
---
## AutoFilter.FilterTop10 method

Filter the top 10 item in the list

```csharp
public void FilterTop10(int fieldIndex, bool isTop, bool isPercent, int itemCount)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| isTop | Boolean | Indicates whether filter from top or bottom |
| isPercent | Boolean | Indicates whether the items is percent or count |
| itemCount | Int32 | The item count |

### Examples

```csharp
// Called: worksheet.AutoFilter.FilterTop10(5, true, false, 5);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "AutoFilter/CellsNet46029.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = "B6:K6";
            worksheet.AutoFilter.FilterTop10(5, true, false, 5);
            worksheet.AutoFilter.Refresh();
            Assert.IsTrue(worksheet.Cells.IsRowHidden(19));
        }
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


