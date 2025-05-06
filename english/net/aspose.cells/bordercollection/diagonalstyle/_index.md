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
[Test]
        public void Property_DiagonalStyle()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellTest01.xlsx&quot;);
            Cells cells = workbook.Worksheets[0].Cells;

            Assert.IsNotNull(cells[&quot;B3&quot;].GetTable());
            Assert.IsTrue(cells[&quot;F2&quot;].IsArrayFormula);
            Assert.IsTrue(cells[&quot;H3&quot;].IsSharedFormula);
            Style style = cells[&quot;F5&quot;].GetStyle();
            Assert.AreEqual(style.Borders.DiagonalStyle, CellBorderType.Thin);
           AssertHelper.AreEqual(style.Borders.DiagonalColor, Color.Red);
        }
```

### See Also

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


