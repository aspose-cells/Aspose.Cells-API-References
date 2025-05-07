---
title: CellsColor.Color
second_title: Aspose.Cells for .NET API Reference
description: CellsColor property. Gets and sets the RGB color
type: docs
url: /net/aspose.cells/cellscolor/color/
---
## CellsColor.Color property

Gets and sets the RGB color.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(m.TransparentColor.Color, Color.White);
[Test]
        public void Property_Color()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA41675.xls");
            Picture pic = workbook.Worksheets[0].Pictures[0];
            MsoFormatPicture m = pic.FormatPicture;
            AssertHelper.AreEqual(m.TransparentColor.Color, Color.White);
        }
```

### See Also

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


