---
title: Row.GroupLevel
second_title: Aspose.Cells for .NET API Reference
description: Row property. Gets the group level of the row
type: docs
url: /net/aspose.cells/row/grouplevel/
---
## Row.GroupLevel property

Gets the group level of the row.

```csharp
public byte GroupLevel { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(2, book.Worksheets[0].Cells.Rows[7].GroupLevel);
[Test]
        public void Property_GroupLevel()
        {
            Workbook book = new Workbook(Constants.sourcePath + @"CELLSNET48621.xlsx");

           Assert.AreEqual(1,book.Worksheets[0].Cells.Rows[2].GroupLevel);
            Assert.AreEqual(2, book.Worksheets[0].Cells.Rows[7].GroupLevel);
            Assert.AreEqual(2, book.Worksheets[0].Cells.Rows[15].GroupLevel);
            book.Save(Constants.destPath + "CELLSNET48621.ods");
            book = new Workbook(Constants.destPath + "CELLSNET48621.ods");
            book.Save(Constants.destPath + "CELLSNET48621.xlsx");
            Assert.AreEqual(1, book.Worksheets[0].Cells.Rows[2].GroupLevel);
            Assert.AreEqual(2, book.Worksheets[0].Cells.Rows[7].GroupLevel);
            Assert.AreEqual(2, book.Worksheets[0].Cells.Rows[15].GroupLevel);
        }
```

### See Also

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


