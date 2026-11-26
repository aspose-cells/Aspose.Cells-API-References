---
title: "TextEffectFormat.Text"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextEffectFormat. Текст в WordArt"
type: docs
url: /ru/net/aspose.cells.drawing/texteffectformat/text/
---
## TextEffectFormat.Text property

Текст в WordArt.

```csharp
public string Text { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyTextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить форму текстового эффекта и установить её текст
            Shape shape = sheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 14, false, false, 0, 0, 0, 0, 100, 100);

            // Получить доступ и изменить свойство текста текстового эффекта
            shape.TextEffect.Text = "Updated Text";

            // Проверить, что текст был обновлён
            Console.WriteLine("Text Effect Content: " + shape.TextEffect.Text);
        }
    }
}
```

### См. также

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


