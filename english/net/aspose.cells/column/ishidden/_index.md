---
title: Column.IsHidden
second_title: Aspose.Cells for .NET API Reference
description: Column property. Indicates whether the column is hidden
type: docs
url: /net/aspose.cells/column/ishidden/
---
## Column.IsHidden property

Indicates whether the column is hidden.

```csharp
public bool IsHidden { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(true, Columns[3].IsHidden);
[Test]
        public void Property_IsHidden()
        {
            Workbook wb = new Workbook(Constants.sourcePath + @&quot;Numbers13\ExpTest\HiddenRowColumn.xlsx&quot;);
#if APPLECHECK
            wb.Save(Constants.sourcePath + @&quot;Numbers13\ExpTest\HiddenRowColumn.numbers&quot;);
#endif
            //wb = new Workbook(Constants.sourcePath + @&quot;Numbers13\ExpTest\HiddenRowColumn.numbers&quot;);
            //wb.Save(Constants.sourcePath + @&quot;Numbers13\ExpTest\HiddenRowColumn-Ret.xlsx&quot;);

            Workbook numbers = Util.ReSave(wb, SaveFormat.Numbers);
            Worksheet worksheet = numbers.Worksheets[0];
            RowCollection rows = worksheet.Cells.Rows;
            Assert.AreEqual(false, rows[21].IsHidden);
            Assert.AreEqual(true, rows[22].IsHidden);
            Assert.AreEqual(true, rows[23].IsHidden);
            worksheet = numbers.Worksheets[1];
            rows = worksheet.Cells.Rows;
            Assert.AreEqual(false, rows[22].IsHidden);
            Assert.AreEqual(true, rows[23].IsHidden);
            Assert.AreEqual(true, rows[24].IsHidden);
            Assert.AreEqual(true, rows[25].IsHidden);
            Assert.AreEqual(false, rows[26].IsHidden);
            //Read Hidden Column is not supported...
            //CELLSNET -58142 -done
            worksheet = numbers.Worksheets[0];
            ColumnCollection Columns = worksheet.Cells.Columns;
            Assert.AreEqual(true, Columns[3].IsHidden);
            Assert.AreEqual(true, Columns[10].IsHidden);
            Assert.AreEqual(false, Columns[11].IsHidden);
            Assert.AreEqual(true, Columns[12].IsHidden);
            Assert.AreEqual(true, Columns[13].IsHidden);
            worksheet = numbers.Worksheets[1];
            Columns = worksheet.Cells.Columns;
            Assert.AreEqual(true, Columns[2].IsHidden);
            Assert.AreEqual(false, Columns[3].IsHidden);
            Assert.AreEqual(true, Columns[7].IsHidden);
            Assert.AreEqual(true, Columns[8].IsHidden);
            Assert.AreEqual(true, Columns[9].IsHidden);
        }
```

### See Also

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


