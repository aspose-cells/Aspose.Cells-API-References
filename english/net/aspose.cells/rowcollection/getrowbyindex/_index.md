---
title: RowCollection.GetRowByIndex
second_title: Aspose.Cells for .NET API Reference
description: RowCollection method. Gets the row object by the position in the list
type: docs
url: /net/aspose.cells/rowcollection/getrowbyindex/
---
## RowCollection.GetRowByIndex method

Gets the row object by the position in the list.

```csharp
public Row GetRowByIndex(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The position. |

### Return Value

The Row object at given position.

### Examples

```csharp
// Called: Assert.AreEqual(33, workbook.Worksheets[0].Cells.Rows.GetRowByIndex(33).Index);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.HtmlPath + &quot;CELLSNET47663.XLSX&quot;);
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            Assert.AreEqual(146, workbook.Worksheets[0].Cells.Rows.Count);
            Assert.AreEqual(0xFFFFF, workbook.Worksheets[0].Cells.Rows.GetRowByIndex(145).Index);
            workbook.Save(_destFilesPath + &quot;CELLSNET47663.html&quot;, saveOptions);
            workbook = new Workbook(_destFilesPath + &quot;CELLSNET47663.html&quot;);
            Assert.AreEqual(34, workbook.Worksheets[0].Cells.Rows.Count);
            Assert.AreEqual(33, workbook.Worksheets[0].Cells.Rows.GetRowByIndex(33).Index);
        }
```

### See Also

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


