---
title: AutoFilter.Range
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter property. Represents the range to which the specified AutoFilter applies
type: docs
url: /net/aspose.cells/autofilter/range/
---
## AutoFilter.Range property

Represents the range to which the specified AutoFilter applies.

```csharp
public string Range { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(sheet.AutoFilter.Range, "A1:A5");
public void AutoFilter_Property_Range()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Worksheet sheet = workbook.Worksheets[0];
    sheet.Cells.DeleteColumns(0,2,false);
    Assert.AreEqual(sheet.AutoFilter.Range, "A1:A5");
}
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


