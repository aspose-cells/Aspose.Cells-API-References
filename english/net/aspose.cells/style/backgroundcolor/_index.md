---
title: Style.BackgroundColor
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets a styles background color
type: docs
url: /net/aspose.cells/style/backgroundcolor/
---
## Style.BackgroundColor property

Gets or sets a style's background color.

```csharp
public Color BackgroundColor { get; set; }
```

### Remarks

If you want to set a cell's color, please use Style.ForegroundColor property. Only if the cell style pattern is other than none or solid, this property will take effect.

### Examples

```csharp
// Called: Assert.IsTrue(cell.GetStyle().BackgroundColor.IsEmpty);
[Test]
        public void Property_BackgroundColor()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet46374.xlsx");
            Cell cell = workbook.Worksheets[0].Cells["E4"];
            Assert.IsTrue(cell.GetStyle().BackgroundColor.IsEmpty);
            workbook.Save(Constants.destPath + "CellsNet46374.xlsx");
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


