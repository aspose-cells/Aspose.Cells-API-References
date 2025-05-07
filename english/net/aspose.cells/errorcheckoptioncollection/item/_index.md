---
title: ErrorCheckOptionCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ErrorCheckOptionCollection property. Gets ErrorCheckOption object by the given index
type: docs
url: /net/aspose.cells/errorcheckoptioncollection/item/
---
## ErrorCheckOptionCollection indexer

Gets [`ErrorCheckOption`](../../errorcheckoption/) object by the given index.

```csharp
public ErrorCheckOption this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index |

### Return Value

Return [`ErrorCheckOption`](../../errorcheckoption/) object

### Examples

```csharp
// Called: int c = workbook.Worksheets[0].ErrorCheckOptions[0].GetCountOfRange();
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET51050.xls");
            int c = workbook.Worksheets[0].ErrorCheckOptions[0].GetCountOfRange();
            workbook.Save(Constants.destPath + "CELLSNET51050.xls");
            workbook = new Workbook(Constants.destPath + "CELLSNET51050.xls");
            Assert.AreEqual(c, workbook.Worksheets[0].ErrorCheckOptions[0].GetCountOfRange());
        }
```

### See Also

* class [ErrorCheckOption](../../errorcheckoption/)
* class [ErrorCheckOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


