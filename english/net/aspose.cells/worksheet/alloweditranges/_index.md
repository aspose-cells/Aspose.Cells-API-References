---
title: Worksheet.AllowEditRanges
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the allow edit range collection in the worksheet
type: docs
url: /net/aspose.cells/worksheet/alloweditranges/
---
## Worksheet.AllowEditRanges property

Gets the allow edit range collection in the worksheet.

```csharp
public ProtectedRangeCollection AllowEditRanges { get; }
```

### Examples

```csharp
// Called: ProtectedRange r = workbook.Worksheets[0].AllowEditRanges[0];
public void Worksheet_Property_AllowEditRanges()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    ProtectedRange r = workbook.Worksheets[0].AllowEditRanges[0];
    Assert.IsTrue(r.IsProtectedWithPassword);
    workbook.Save(Constants.destPath + "example.xlsb");
    workbook = new Workbook(Constants.destPath + "example.xlsb");
    Assert.IsTrue(r.IsProtectedWithPassword);

}
```

### See Also

* class [ProtectedRangeCollection](../../protectedrangecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


