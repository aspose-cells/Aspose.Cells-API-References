---
title: Cells.HideGroupDetail
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Collapses the grouped rows/columns
type: docs
url: /net/aspose.cells/cells/hidegroupdetail/
---
## Cells.HideGroupDetail method

Collapses the grouped rows/columns.

```csharp
public void HideGroupDetail(bool isVertical, int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isVertical | Boolean | True, collapse the grouped rows. |
| index | Int32 | The row/column index |

### Examples

```csharp
// Called: worksheet.Cells.HideGroupDetail(true, 7);
public void Cells_Method_HideGroupDetail()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var worksheet = workbook.Worksheets["Sheet1"];

    worksheet.Cells.HideGroupDetail(true, 4);
    worksheet.Cells.HideGroupDetail(true, 7);
    Console.WriteLine(DateTime.Now);
    workbook.Save(Constants.destPath + "example.xlsx");
    bool c = ManualFileUtil.ManualCheckStringInZip(Constants.destPath + @"example.xlsx", "xl/worksheets/sheet1.xml", new string[] { "collapsed=\"1\"" }, true);
    Assert.IsTrue(c);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


