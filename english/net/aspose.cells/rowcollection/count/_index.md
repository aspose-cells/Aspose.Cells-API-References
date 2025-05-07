---
title: RowCollection.Count
second_title: Aspose.Cells for .NET API Reference
description: RowCollection property. Gets the number of rows in this collection
type: docs
url: /net/aspose.cells/rowcollection/count/
---
## RowCollection.Count property

Gets the number of rows in this collection.

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(146, workbook.Worksheets[0].Cells.Rows.Count);
[Test]
        public void Property_Count()
        {
            Workbook workbook = new Workbook(Constants.HtmlPath + "CELLSNET47663.XLSX");
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            Assert.AreEqual(146, workbook.Worksheets[0].Cells.Rows.Count);
            Assert.AreEqual(0xFFFFF, workbook.Worksheets[0].Cells.Rows.GetRowByIndex(145).Index);
            workbook.Save(_destFilesPath + "CELLSNET47663.html", saveOptions);
            workbook = new Workbook(_destFilesPath + "CELLSNET47663.html");
            Assert.AreEqual(34, workbook.Worksheets[0].Cells.Rows.Count);
            Assert.AreEqual(33, workbook.Worksheets[0].Cells.Rows.GetRowByIndex(33).Index);
        }
```

### See Also

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


