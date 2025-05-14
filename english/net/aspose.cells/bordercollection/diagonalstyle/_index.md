---
title: BorderCollection.DiagonalStyle
second_title: Aspose.Cells for .NET API Reference
description: BorderCollection property. Gets or sets the style of Diagonal lines
type: docs
url: /net/aspose.cells/bordercollection/diagonalstyle/
---
## BorderCollection.DiagonalStyle property

Gets or sets the style of Diagonal lines.

```csharp
public CellBorderType DiagonalStyle { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(style.Borders.DiagonalStyle, CellBorderType.Thin);
public void BorderCollection_Property_DiagonalStyle()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Cells cells = workbook.Worksheets[0].Cells;

    Assert.IsNotNull(cells["B3"].GetTable());
    Assert.IsTrue(cells["F2"].IsArrayFormula);
    Assert.IsTrue(cells["H3"].IsSharedFormula);
    Style style = cells["F5"].GetStyle();
    Assert.AreEqual(style.Borders.DiagonalStyle, CellBorderType.Thin);
   AssertHelper.AreEqual(style.Borders.DiagonalColor, Color.Red);
}
```

### See Also

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


