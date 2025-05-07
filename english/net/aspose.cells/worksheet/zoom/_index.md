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
// Called: Assert.AreEqual(100, workbook.Worksheets[0].Zoom);
[Test]
        public void Property_Zoom()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet44478.xlsx");
            Assert.AreEqual(100, workbook.Worksheets[0].Zoom);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


