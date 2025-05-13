---
title: Column.Width
second_title: Aspose.Cells for .NET API Reference
description: Column property. Gets and sets the column width in unit of characters
type: docs
url: /net/aspose.cells/column/width/
---
## Column.Width property

Gets and sets the column width in unit of characters.

```csharp
public double Width { get; set; }
```

### Remarks

For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.

### Examples

```csharp
// Called: columnsWidth = numbers.Worksheets[0].Cells.Columns[3].Width;
public void Column_Property_Width()
{
    //Numbers35SaveOptions op = new Numbers35SaveOptions();
    Workbook wb = new Workbook(Constants.sourcePath + @"example.xlsx");
    //Workbook numbers = Util.ReSave(wb, SaveFormat.Numbers);
    //wb.Save(Constants.sourcePath + @"example.numbers",op);
    Workbook numbers = Util.ReSave(wb, SaveFormat.Numbers);
    double rowHeight = numbers.Worksheets[0].Cells.Rows[2].Height;
    Assert.AreEqual(19.95, rowHeight);
    rowHeight = numbers.Worksheets[0].Cells.Rows[3].Height;
    Assert.AreEqual(58.8, rowHeight);

    rowHeight = numbers.Worksheets[1].Cells.Rows[1].Height;
    Assert.AreEqual(19.95, rowHeight);
    rowHeight = numbers.Worksheets[1].Cells.Rows[2].Height;
    Assert.AreEqual(73.2, rowHeight);

    double columnsWidth = numbers.Worksheets[0].Cells.Columns[2].Width;
    Assert.AreEqual(18, columnsWidth);
    columnsWidth = numbers.Worksheets[0].Cells.Columns[3].Width;
    Assert.AreEqual(51.43, columnsWidth);

    columnsWidth = numbers.Worksheets[1].Cells.Columns[1].Width;
    Assert.AreEqual(18, columnsWidth);
    columnsWidth = numbers.Worksheets[1].Cells.Columns[2].Width;
    Assert.AreEqual(46.14, columnsWidth);

}
```

### See Also

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


