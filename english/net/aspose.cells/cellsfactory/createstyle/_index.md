---
title: CellsFactory.CreateStyle
second_title: Aspose.Cells for .NET API Reference
description: CellsFactory method. Creates a new style
type: docs
url: /net/aspose.cells/cellsfactory/createstyle/
---
## CellsFactory.CreateStyle method

Creates a new style.

```csharp
public Style CreateStyle()
```

### Return Value

Returns a style object.

### Examples

```csharp
// Called: Style style = new CellsFactory().CreateStyle();
[Test]
        public void Method_CreateStyle()
        {
            Workbook wb = new Workbook();
            Style style = new CellsFactory().CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            wb.Worksheets[0].Cells.CreateRange(0, 1, false).SetStyle(style, true);
           Assert.IsTrue( wb.Worksheets[0].Cells.Rows[0].GetCellOrNull(3) == null);
            wb.Save(Constants.destPath + &quot;CELLSNET57109.xlsx&quot;);
        }
```

### See Also

* class [Style](../../style/)
* class [CellsFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


