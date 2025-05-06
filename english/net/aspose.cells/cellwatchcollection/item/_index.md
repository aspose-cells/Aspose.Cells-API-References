---
title: CellWatchCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: CellWatchCollection property. Gets and sets CellWatch by index
type: docs
url: /net/aspose.cells/cellwatchcollection/item/
---
## CellWatchCollection indexer (1 of 2)

Gets and sets [`CellWatch`](../../cellwatch/) by index.

```csharp
public CellWatch this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;F9&amp;quot;,workbook.Worksheets[1].CellWatches[0].CellName);
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA42625.xlsx&quot;);
            Assert.AreEqual(2, workbook.Worksheets[1].CellWatches.Count);
            Assert.AreEqual(&quot;F9&quot;,workbook.Worksheets[1].CellWatches[0].CellName);
            workbook.Worksheets[1].CellWatches.Add(&quot;A1&quot;);
            workbook.Save(Constants.destPath + &quot;CELLSJAVA42625.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSJAVA42625.xlsx&quot;);
            Assert.AreEqual(3, workbook.Worksheets[1].CellWatches.Count);
        }
```

### See Also

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CellWatchCollection indexer (2 of 2)

Gets and sets [`CellWatch`](../../cellwatch/) by the name of the cell.

```csharp
public CellWatch this[string cellName] { get; }
```

| Parameter | Description |
| --- | --- |
| cellName | The name of the cell. |

### See Also

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


