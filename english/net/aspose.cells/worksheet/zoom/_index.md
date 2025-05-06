---
title: Worksheet.Zoom
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents the scaling factor in percentage. It should be between 10 and 400
type: docs
url: /net/aspose.cells/worksheet/zoom/
---
## Worksheet.Zoom property

Represents the scaling factor in percentage. It should be between 10 and 400.

```csharp
public int Zoom { get; set; }
```

### Remarks

Please set the view type first.

### Examples

```csharp
// Called: Assert.AreEqual(200, workbook.Worksheets[0].Zoom);
[Test]
        public void Property_Zoom()
        {
            Workbook workbook = new Workbook(Constants.HtmlSourcePath + &quot;Cellsjava45029.htm&quot;);
            Assert.AreEqual(200, workbook.Worksheets[0].Zoom);
            int row, col, rows, cols;
            workbook.Worksheets[0].GetFreezedPanes(out row, out col, out rows, out cols);
            Assert.AreEqual(row, 1);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


