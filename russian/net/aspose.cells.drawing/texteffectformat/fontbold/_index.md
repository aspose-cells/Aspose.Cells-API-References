---
title: "TextEffectFormat.FontBold"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextEffectFormat. Указывает, является ли шрифт полужирным"
type: docs
url: /ru/net/aspose.cells.drawing/texteffectformat/fontbold/
---
## TextEffectFormat.FontBold property

Указывает, является ли шрифт полужирным.

```csharp
public bool FontBold { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontBoldDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму текстового поля (возвращает объект TextBox напрямую)
            TextBox textbox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 200, 100);
            textbox.Text = "Sample Text";

            // Получить формат текстового эффекта
            TextEffectFormat effFormat = textbox.TextEffect;

            // Установить свойства шрифта, включая полужирный
            effFormat.FontName = "Arial";
            effFormat.FontBold = true;
            effFormat.FontItalic = false;
            effFormat.FontSize = 14;

            // Сохраните книгу
            workbook.Save("TextEffectFormatFontBoldDemo.xlsx");

            Console.WriteLine("Text effect format with bold font applied successfully.");
        }
    }
}
```

### См. также

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


