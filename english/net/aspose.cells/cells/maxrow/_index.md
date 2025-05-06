---
title: Cells.MaxRow
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Maximum row index of cell which contains data or style
type: docs
url: /net/aspose.cells/cells/maxrow/
---
## Cells.MaxRow property

Maximum row index of cell which contains data or style.

```csharp
public int MaxRow { get; }
```

### Remarks

Return -1 if there is no cell which contains data or style in the worksheet.

### Examples

```csharp
// Called: Assert.AreEqual(340, book.Worksheets[0].Cells.MaxRow);
[Test]
        public void Property_MaxRow()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA41873/&quot;;

            Workbook book = new Workbook(filePath + &quot;WCQX_Pusheen.xls&quot;);
            Console.WriteLine(book.Worksheets[0].Cells.MaxDisplayRange.RowCount + &quot;     &quot; + book.Worksheets[0].Cells.MaxDisplayRange.ColumnCount);
            addEmptyColumn(book);
            addColRowHeader(book);
            addColRowHeaderStyle(book);
            fixCellStyle(book);

            for (int i = 0; i &lt; book.Worksheets.Count; i++)
            {
                if (i != 0)
                {
                    book.Worksheets[i].IsVisible = false;
                }
            }
            Console.WriteLine(book.Worksheets[0].Cells.MaxDisplayRange.RowCount + &quot;     &quot; + book.Worksheets[0].Cells.MaxDisplayRange.ColumnCount);
            book.Save(CreateFolder(filePath) + &quot;out.xls&quot;);
            HtmlSaveOptions saveOps = new HtmlSaveOptions();
            saveOps.ExportHiddenWorksheet = false;

            book.Save(Constants.destPath + &quot;JAVA41873.html&quot;, saveOps);
            book = new Workbook(Constants.destPath + &quot;JAVA41873.html&quot;);
            Assert.AreEqual(340, book.Worksheets[0].Cells.MaxRow);
            Assert.AreEqual(16, book.Worksheets[0].Cells.MaxColumn);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


