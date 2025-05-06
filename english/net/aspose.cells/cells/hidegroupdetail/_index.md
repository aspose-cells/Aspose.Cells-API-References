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
// Called: worksheet.Cells.HideGroupDetail(false, 4);
[Test]
        public void  Method_Int32_()
        {
            var workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET50038.xlsx&quot;);
            var worksheet = workbook.Worksheets[&quot;Sheet1&quot;];

            worksheet.Cells.HideGroupDetail(false, 4);
            worksheet.Cells.HideGroupDetail(false, 7);
            MemoryStream ms = Util.SaveAsBuffer(workbook, SaveFormat.Xlsx);
            bool c =ManualFileUtil.ManualCheckStringInZip(ms, &quot;xl/worksheets/sheet1.xml&quot;,
                new string[] { &quot;collapsed=\&quot;1\&quot;&quot; }, true);
            Assert.IsTrue(c);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


