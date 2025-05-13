---
title: Worksheet.ErrorCheckOptions
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets error check setting applied on certain ranges
type: docs
url: /net/aspose.cells/worksheet/errorcheckoptions/
---
## Worksheet.ErrorCheckOptions property

Gets error check setting applied on certain ranges.

```csharp
public ErrorCheckOptionCollection ErrorCheckOptions { get; }
```

### Examples

```csharp
// Called: int c = workbook.Worksheets[0].ErrorCheckOptions[0].GetCountOfRange();
public void Worksheet_Property_ErrorCheckOptions()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    int c = workbook.Worksheets[0].ErrorCheckOptions[0].GetCountOfRange();
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    Assert.AreEqual(c, workbook.Worksheets[0].ErrorCheckOptions[0].GetCountOfRange());
}
```

### See Also

* class [ErrorCheckOptionCollection](../../errorcheckoptioncollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


