---
title: Worksheet.AutoFilter
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents auto filter for the specified worksheet
type: docs
url: /net/aspose.cells/worksheet/autofilter/
---
## Worksheet.AutoFilter property

Represents auto filter for the specified worksheet.

```csharp
public AutoFilter AutoFilter { get; }
```

### Examples

```csharp
// Called: worksheet.AutoFilter.Refresh();
public void Worksheet_Property_AutoFilter()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];
    worksheet.AutoFilter.Range = "B6:K6";
    worksheet.AutoFilter.FilterTop10(5, true, false, 5);
    worksheet.AutoFilter.Refresh();
    Assert.IsTrue(worksheet.Cells.IsRowHidden(19));
}
```

### See Also

* class [AutoFilter](../../autofilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


