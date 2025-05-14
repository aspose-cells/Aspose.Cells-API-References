---
title: Border.LineStyle
second_title: Aspose.Cells for .NET API Reference
description: Border property. Gets or sets the cell border type
type: docs
url: /net/aspose.cells/border/linestyle/
---
## Border.LineStyle property

Gets or sets the cell border type.

```csharp
public CellBorderType LineStyle { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(CellBorderType.None, style.Borders[BorderType.BottomBorder].LineStyle);
public void Border_Property_LineStyle()
{
    Workbook workbook = new Workbook(Constants.HtmlSourcePath + "example.xlsx");
    workbook.Save(Constants.HtmlDestPath + "example.html");
    workbook = new Workbook(Constants.HtmlDestPath + "example.html");
    Cell cell = workbook.Worksheets[0].Cells["B14"];
    Style style = cell.GetStyle(true);
    workbook.Save(Constants.HtmlDestPath + "example.xlsx");
    Assert.AreEqual(CellBorderType.None, style.Borders[BorderType.BottomBorder].LineStyle);
}
```

### See Also

* enum [CellBorderType](../../cellbordertype/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


