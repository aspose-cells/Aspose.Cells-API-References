---
title: "StyleFlag.Font"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Yazı tipi ayarları uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/font/
---
## StyleFlag.Font property

Yazı tipi ayarları uygulanacak.

```csharp
public bool Font { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


