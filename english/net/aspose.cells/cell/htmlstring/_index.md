---
title: Cell.HtmlString
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets and sets the html string which contains data and some formats in this cell
type: docs
url: /net/aspose.cells/cell/htmlstring/
---
## Cell.HtmlString property

Gets and sets the html string which contains data and some formats in this cell.

```csharp
public string HtmlString { get; set; }
```

### Examples

```csharp
// Called: cells["A1"].HtmlString = "I am <br/>a <i>strValue</i> value.";
public void Cell_Property_HtmlString()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Style style = cells["A1"].GetStyle();
    style.Font.IsBold = true;
    cells["A1"].SetStyle(style);

    cells["A1"].HtmlString = "I am <br/>a <i>strValue</i> value.";
    Assert.IsTrue(cells["A1"].StringValue.IndexOf('\n') != -1);
    workbook.Save(Constants.destPath + "XlsSave.xls", new XlsSaveOptions());
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


