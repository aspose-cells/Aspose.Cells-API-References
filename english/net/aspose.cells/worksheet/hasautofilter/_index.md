---
title: Worksheet.HasAutofilter
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates whether this worksheet has auto filter
type: docs
url: /net/aspose.cells/worksheet/hasautofilter/
---
## Worksheet.HasAutofilter property

Indicates whether this worksheet has auto filter.

```csharp
public bool HasAutofilter { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].HasAutofilter);
public void Worksheet_Property_HasAutofilter()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");
    Assert.IsTrue(workbook.Worksheets[0].HasAutofilter);
    workbook.Save(Constants.destPath + "example.xlsx");
            
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


