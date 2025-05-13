---
title: BorderCollection.SetStyle
second_title: Aspose.Cells for .NET API Reference
description: BorderCollection method. Sets the style of all borders of the collection
type: docs
url: /net/aspose.cells/bordercollection/setstyle/
---
## BorderCollection.SetStyle method

Sets the style of all borders of the collection.

```csharp
public void SetStyle(CellBorderType style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | CellBorderType | Borders' style |

### Examples

```csharp
// Called: s.Borders.SetStyle(CellBorderType.Thick);
// http://www.aspose.com/community/forums/thread/256893/unable-to-change-borders-on-cells.aspx
public void BorderCollection_Method_SetStyle()
{
    Console.WriteLine("BorderCollection_Method_SetStyle()");
    string infn = path + "Test_ChangeCellBorder.xlsm";
    string outfn = Constants.destPath + "Test_ChangeCellBorder_out.xlsm";

    Workbook book = new Workbook(infn);
    Worksheet ws = book.Worksheets[5];
    Style s = ws.Cells["C6"].GetStyle();
    s.Borders.SetColor(System.Drawing.Color.Red);
    s.Borders.SetStyle(CellBorderType.Thick);
    ws.Cells["C6"].SetStyle(s);
    book.Save(outfn);

    Workbook book1 = new Workbook(outfn);
    Worksheet ws1 = book1.Worksheets[5];
    Style s1 = ws1.Cells["C6"].GetStyle();

    BorderCollection bds = s1.Borders;
    Test_ChangeCellBorder_checkBorderStyle(bds[BorderType.BottomBorder]);
    Test_ChangeCellBorder_checkBorderStyle(bds[BorderType.LeftBorder]);
    Test_ChangeCellBorder_checkBorderStyle(bds[BorderType.RightBorder]);
    Test_ChangeCellBorder_checkBorderStyle(bds[BorderType.TopBorder]);
    Test_ChangeCellBorder_checkBorderStyle(bds[BorderType.DiagonalDown]);
    //Test_ChangeCellBorder_checkBorderStyle(bds[BorderType.DiagonalUp]);

}
```

### See Also

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


