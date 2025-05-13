---
title: FormatConditionCollection.AddArea
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection method. Adds a conditional formatted cell range
type: docs
url: /net/aspose.cells/formatconditioncollection/addarea/
---
## FormatConditionCollection.AddArea method

Adds a conditional formatted cell range.

```csharp
public int AddArea(CellArea cellArea)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Conditional formatted cell range. |

### Return Value

Conditional formatted cell rang index.

### Examples

```csharp
// Called: formatCollection.AddArea(area);
public void FormatConditionCollection_Method_AddArea()
{
    Workbook wk = new Workbook(Constants.sourcePath + "example.xlsx");
    DateTime dt = DateTime.Now;
    ConditionalFormattingCollection asposeFormattingCollection = wk.Worksheets[0].ConditionalFormattings;

    //long start = System.currentTimeMillis();
    for (int row = 16; row < 3000; row++)
    {
        for (int col = 2; col < 12; col++)
        {
            FormatConditionCollection formatCollection = asposeFormattingCollection[0];
            formatCollection.RemoveArea(row, col, 1, 1);
            CellArea area = CellArea.CreateCellArea(row, col, row, col);
            formatCollection.AddArea(area);
        }
    }
    Assert.AreEqual(2,asposeFormattingCollection[0].RangeCount);
}
```

### See Also

* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


