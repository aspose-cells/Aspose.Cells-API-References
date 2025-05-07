---
title: HorizontalPageBreakCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: HorizontalPageBreakCollection property. Gets the HorizontalPageBreak element at the specified index
type: docs
url: /net/aspose.cells/horizontalpagebreakcollection/item/
---
## HorizontalPageBreakCollection indexer (1 of 2)

Gets the [`HorizontalPageBreak`](../../horizontalpagebreak/) element at the specified index.

```csharp
public HorizontalPageBreak this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Assert.AreEqual(12, breaks[1].Row);
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET48675.xlsx");
            HorizontalPageBreakCollection breaks = workbook.Worksheets[0].HorizontalPageBreaks;
            Assert.AreEqual(2, breaks.Count);
            Assert.AreEqual(6, breaks[0].Row);
            Assert.AreEqual(12, breaks[1].Row);
            workbook.Save(Constants.destPath + "CELLSNET48675.ods");
            workbook = new Workbook(Constants.destPath + "CELLSNET48675.ods");
             breaks = workbook.Worksheets[0].HorizontalPageBreaks;
            Assert.AreEqual(2, breaks.Count);
            Assert.AreEqual(6, breaks[0].Row);
            Assert.AreEqual(12, breaks[1].Row);
            workbook.Save(Constants.destPath + "CELLSNET48675.xlsx");
        }
```

### See Also

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HorizontalPageBreakCollection indexer (2 of 2)

Gets the [`HorizontalPageBreak`](../../horizontalpagebreak/) element with the specified cell name.

```csharp
public HorizontalPageBreak this[string cellName] { get; }
```

| Parameter | Description |
| --- | --- |
| cellName | Cell name. |

### Return Value

The element with the specified cell name.

### See Also

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


