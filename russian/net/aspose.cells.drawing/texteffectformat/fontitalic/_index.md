---
title: "TextEffectFormat.FontItalic"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextEffectFormat. Указывает, курсивен ли шрифт"
type: docs
url: /ru/net/aspose.cells.drawing/texteffectformat/fontitalic/
---
## TextEffectFormat.FontItalic property

Указывает, является ли шрифт курсивом.

```csharp
public bool FontItalic { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontItalicDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму с текстовым эффектом
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 0, 0, 100, 100);

            // Получить формат текстового эффекта
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Установить FontItalic в true
            textEffectFormat.FontItalic = true;
            Console.WriteLine("FontItalic after setting to true: " + textEffectFormat.FontItalic);

            // Установить FontItalic в false
            textEffectFormat.FontItalic = false;
            Console.WriteLine("FontItalic after setting to false: " + textEffectFormat.FontItalic);

            // Сохраните книгу
            workbook.Save("TextEffectFormatFontItalicDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


