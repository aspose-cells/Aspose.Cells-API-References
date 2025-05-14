---
title: StyleFlag.Font
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Font settings will be applied
type: docs
url: /net/aspose.cells/styleflag/font/
---
## StyleFlag.Font property

Font settings will be applied.

```csharp
public bool Font { get; set; }
```

### Examples

```csharp
// Called: flag.Font = true;
public void StyleFlag_Property_Font()
{
    Workbook workbook = new Workbook();
    ShapeCollection shapes = workbook.Worksheets[0].Shapes;
    Button shape = shapes.AddButton(0, 0, 0, 0, 100, 100);
    shape.Text = "sdfsdfsdfsdf";
    Aspose.Cells.Font font = workbook.CreateStyle().Font;
    font.Color = Color.Red;
    StyleFlag flag = new StyleFlag();
    flag.Font = true;
    shape.FormatCharacters(0, shape.Text.Length, font, flag);
    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


