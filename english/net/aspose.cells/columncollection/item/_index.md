---
title: ColumnCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ColumnCollection property. Gets a Column object by column index. The Column object of given column index will be instantiated if it does not exist before
type: docs
url: /net/aspose.cells/columncollection/item/
---
## ColumnCollection indexer

Gets a [`Column`](../../column/) object by column index. The Column object of given column index will be instantiated if it does not exist before.

```csharp
public Column this[int columnIndex] { get; }
```

### Examples

```csharp
// Called: Assert.Less(columns[0].Width, 12);
public void ColumnCollection_Property_Item()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47034/";

    Aspose.Cells.HtmlLoadOptions options = new Aspose.Cells.HtmlLoadOptions(Aspose.Cells.LoadFormat.Html);

    options.AutoFitColsAndRows = true;
    options.AutoFitterOptions = new AutoFitterOptions
    {
        AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
    };
    options.SetPaperSize(PaperSizeType.PaperA4);

    Workbook workbook = new Workbook(filePath + "test.html", options);
    workbook.Save(CreateFolder(filePath) + @"out.xls", Aspose.Cells.SaveFormat.Excel97To2003);
    ColumnCollection columns = workbook.Worksheets[0].Cells.Columns;
    //Assert.Greater(columns[0].Width, 19d);
    //Assert.Greater(columns[1].Width, 19d);
    //Assert.Greater(columns[2].Width, 19d);
    //Assert.Greater(columns[3].Width, 19d);
    //error, just pass
    Assert.Less(columns[0].Width, 12);
    Assert.Less(columns[1].Width, 12);
    Assert.Less(columns[2].Width, 12);
    Assert.Less(columns[3].Width, 12);

}
```

### See Also

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


