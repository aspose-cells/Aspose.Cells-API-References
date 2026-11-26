---
title: "TextEffectFormat.RotatedChars"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextEffectFormat. Если true, символы в указанном WordArt вращаются на 90 градусов относительно ограничивающей формы WordArt"
type: docs
url: /ru/net/aspose.cells.drawing/texteffectformat/rotatedchars/
---
## TextEffectFormat.RotatedChars property

Если true, символы в указанном WordArt вращаются на 90 градусов относительно ограничивающей формы WordArt.

```csharp
public bool RotatedChars { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyRotatedCharsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму с текстовым эффектом
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 100, 100, 200, 50);

            // Получить формат текстового эффекта
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Установить свойство RotatedChars в true
            textEffectFormat.RotatedChars = true;

            // Сохраните книгу
            workbook.Save("TextEffectFormat_RotatedChars_Output.xlsx");

            // Проверить свойство RotatedChars
            Console.WriteLine("RotatedChars property value: " + textEffectFormat.RotatedChars);
        }
    }
}
```

### См. также

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


