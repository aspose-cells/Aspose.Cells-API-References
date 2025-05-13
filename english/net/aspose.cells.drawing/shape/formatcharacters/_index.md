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
// Called: tb.FormatCharacters(0, tb.Text.Length, font, flag);
public void Shape_Method_FormatCharacters()
{
    Workbook workbook = new Workbook();
    TextBox tb = workbook.Worksheets[0].Shapes.AddTextBox(0, 0, 0, 0, 100, 100);
    tb.Text = "sd\nsdfsdfsd";

    tb.Characters(0, 1).Font.IsSuperscript = true;
    Aspose.Cells.Font font = tb.Font;


    font.Size = 7;
    font.Name = "Meiryo UI";
    StyleFlag flag = new StyleFlag();
    flag.FontSize = true;
    flag.FontName = true;
    tb.FormatCharacters(0, tb.Text.Length, font, flag);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    tb = workbook.Worksheets[0].TextBoxes[0];
    Assert.AreEqual("Meiryo UI", tb.Characters(4, 3).Font.Name);
}
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


