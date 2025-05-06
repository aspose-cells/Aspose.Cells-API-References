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
// Called: AssertHelper.AreEqual(Color.White,shapes[0].FormatPicture.TransparentColor.Color);
[Test]
        public void Property_Color()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsJava42980.XLSX&quot;);
            Picture picture = workbook.Worksheets[0].Pictures[3];
            //workbook.Save(dir + &quot;dest.xlsx&quot;);
            Workbook w = new Workbook();
            ShapeCollection shapes = w.Worksheets[0].Shapes;
            shapes.AddCopy(picture, 0, 0, 0, 0);
            w.Save(Constants.destPath + &quot;CellsJava42980.xlsx&quot;);
            AssertHelper.AreEqual(Color.White,shapes[0].FormatPicture.TransparentColor.Color);
           

        }
```

### See Also

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


