---
title: Shape.FormatCharacters
second_title: Aspose.Cells for .NET API Reference
description: Shape method. Formats some characters with the font setting
type: docs
url: /net/aspose.cells.drawing/shape/formatcharacters/
---
## Shape.FormatCharacters method

Formats some characters with the font setting.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | The start index. |
| length | Int32 | The length. |
| font | Font | The font setting. |
| flag | StyleFlag | The flag of the font setting. |

### Examples

```csharp
// Called: shape.FormatCharacters(0, shape.Text.Length, font, flag);
[Test]
        public void Method_StyleFlag_()
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
            workbook.Save(Constants.destPath + "CELLSJAVA40250.xls");
        }
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


