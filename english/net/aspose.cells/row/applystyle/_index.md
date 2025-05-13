---
title: Row.ApplyStyle
second_title: Aspose.Cells for .NET API Reference
description: Row method. Applies formats for a whole row
type: docs
url: /net/aspose.cells/row/applystyle/
---
## Row.ApplyStyle method

Applies formats for a whole row.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### Examples

```csharp
// Called: row.ApplyStyle(style, new StyleFlag { WrapText = true });
public void Row_Method_ApplyStyle()
{
    var workbook = new Workbook();
    var sheet = workbook.Worksheets[0];
    var cell = sheet.Cells[0, 0];

    var input = @"<font style=""color: #49c131; font-weight: bold;"">First </font><font>row</font><br /><font style=""color: #ff7f50; font-weight: bold;"">Second </font><font>row</font>";

    cell.HtmlString = input;

    var row = sheet.Cells.Rows[0];
    var style = row.GetStyle();
    style.IsTextWrapped = true;
    row.ApplyStyle(style, new StyleFlag { WrapText = true });

    sheet.AutoFitRows();
    sheet.AutoFitColumns();

    Assert.AreEqual(61, sheet.Cells.GetColumnWidthPixel(0));
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


