---
title: RangeCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: RangeCollection method. Adds a Range item to the collection
type: docs
url: /net/aspose.cells/rangecollection/add/
---
## RangeCollection.Add method

Adds a [`Range`](../../range/) item to the collection.

```csharp
public int Add(Range range)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Range object |

### Examples

```csharp
// Called: worksheet.Cells.Ranges.Add(cellRange);
[Test]
        public void Method_Range_()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            worksheet.Cells.InsertRows(2, 2, true);
            Assert.AreEqual(5, cellRange.RowCount);
        }
```

### See Also

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


