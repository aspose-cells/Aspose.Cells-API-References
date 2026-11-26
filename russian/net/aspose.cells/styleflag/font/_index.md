---
title: "StyleFlag.Font"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройки шрифта будут применены"
type: docs
url: /ru/net/aspose.cells/styleflag/font/
---
## StyleFlag.Font property

Настройки шрифта будут применены.

```csharp
public bool Font { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var shape = workbook.Worksheets[0].Shapes.AddButton(0, 0, 100, 100, 100, 100);
            shape.Text = "Sample Text";
            
            Aspose.Cells.Font font = workbook.CreateStyle().Font;
            font.Name = "Arial";
            font.Size = 14;
            font.Color = Color.Blue;
            font.IsBold = true;
            
            StyleFlag flag = new StyleFlag();
            flag.Font = true;
            
            shape.FormatCharacters(0, shape.Text.Length, font, flag);
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


