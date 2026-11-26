---
title: "TextEffectFormat.FontName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextEffectFormat. Имя шрифта, используемого в WordArt"
type: docs
url: /ru/net/aspose.cells.drawing/texteffectformat/fontname/
---
## TextEffectFormat.FontName property

Имя шрифта, используемого в WordArt.

```csharp
public string FontName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму WordArt
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 0, 0, 100, 100);

            // Установить и получить свойство FontName
            shape.TextEffect.FontName = "+mn-ea";
            string fontName = shape.TextEffect.FontName;

            // Вывести результат.
            Console.WriteLine("Font Name: " + fontName);
        }
    }
}
```

### См. также

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


