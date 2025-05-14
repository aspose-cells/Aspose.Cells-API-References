---
title: Worksheet.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents if the worksheet is visible
type: docs
url: /net/aspose.cells/worksheet/isvisible/
---
## Worksheet.IsVisible property

Represents if the worksheet is visible.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
// Called: book.Worksheets[i].IsVisible = false;
public void Worksheet_Property_IsVisible()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA41873/";

    Workbook book = new Workbook(filePath + "WCQX_Pusheen.xls");
    Console.WriteLine(book.Worksheets[0].Cells.MaxDisplayRange.RowCount + "     " + book.Worksheets[0].Cells.MaxDisplayRange.ColumnCount);
    addEmptyColumn(book);
    addColRowHeader(book);
    addColRowHeaderStyle(book);
    fixCellStyle(book);

    for (int i = 0; i < book.Worksheets.Count; i++)
    {
        if (i != 0)
        {
            book.Worksheets[i].IsVisible = false;
        }
    }
    Console.WriteLine(book.Worksheets[0].Cells.MaxDisplayRange.RowCount + "     " + book.Worksheets[0].Cells.MaxDisplayRange.ColumnCount);
    book.Save(CreateFolder(filePath) + "out.xls");
    HtmlSaveOptions saveOps = new HtmlSaveOptions();
    saveOps.ExportHiddenWorksheet = false;

    book.Save(Constants.destPath + "example.html", saveOps);
    book = new Workbook(Constants.destPath + "example.html");
    Assert.AreEqual(340, book.Worksheets[0].Cells.MaxRow);
    Assert.AreEqual(16, book.Worksheets[0].Cells.MaxColumn);
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


