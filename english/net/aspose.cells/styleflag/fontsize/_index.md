---
title: StyleFlag.FontSize
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Font size setting will be applied
type: docs
url: /net/aspose.cells/styleflag/fontsize/
---
## StyleFlag.FontSize property

Font size setting will be applied.

```csharp
public bool FontSize { get; set; }
```

### Examples

```csharp
// Called: flag.FontSize = true;
[Test]
        public void Property_FontSize()
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
            workbook.Save(Constants.destPath + "CellsNet53357.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet53357.xlsx");
            tb = workbook.Worksheets[0].TextBoxes[0];
            Assert.AreEqual("Meiryo UI", tb.Characters(4, 3).Font.Name);
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


