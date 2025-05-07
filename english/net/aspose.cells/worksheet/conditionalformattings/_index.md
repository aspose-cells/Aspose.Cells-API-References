---
title: Worksheet.ConditionalFormattings
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the ConditionalFormattings in the worksheet
type: docs
url: /net/aspose.cells/worksheet/conditionalformattings/
---
## Worksheet.ConditionalFormattings property

Gets the ConditionalFormattings in the worksheet.

```csharp
public ConditionalFormattingCollection ConditionalFormattings { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(2, workbook.Worksheets[0].ConditionalFormattings[0].GetCellArea(0).EndRow);
[Test]
        public void Property_ConditionalFormattings()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet41678.xlsx");
            ListObject table = workbook.Worksheets[0].ListObjects[0];
            table.Resize(0, 0, 2, 1, true);
            Assert.AreEqual(2, workbook.Worksheets[0].ConditionalFormattings[0].GetCellArea(0).EndRow);
            workbook.Save(Constants.destPath + "CellsNet41678.xlsx");
        }
```

### See Also

* class [ConditionalFormattingCollection](../../conditionalformattingcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


