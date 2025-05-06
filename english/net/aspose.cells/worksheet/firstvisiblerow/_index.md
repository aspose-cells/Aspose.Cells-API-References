---
title: Worksheet.FirstVisibleRow
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents first visible row index
type: docs
url: /net/aspose.cells/worksheet/firstvisiblerow/
---
## Worksheet.FirstVisibleRow property

Represents first visible row index.

```csharp
public int FirstVisibleRow { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, workbook.Worksheets[0].FirstVisibleRow);
[Test]
        public void Property_FirstVisibleRow()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.HideColumn(0);
            cells.HideRow(0);
            Assert.AreEqual(1, workbook.Worksheets[0].FirstVisibleRow);
            Assert.AreEqual(1, workbook.Worksheets[0].FirstVisibleColumn);
            workbook.Save(Constants.destPath + &quot;CELLSJAVA42631.xlsx&quot;);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


