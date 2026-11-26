---
title: "TextEffectFormat.FontSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextEffectFormat. Размер шрифта в пунктах, используемого в WordArt"
type: docs
url: /ru/net/aspose.cells.drawing/texteffectformat/fontsize/
---
## TextEffectFormat.FontSize property

Размер (в пунктах) шрифта, используемого в WordArt.

```csharp
public int FontSize { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            int textboxIndex = worksheet.TextBoxes.Add(5, 5, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[textboxIndex];
            
            // Установить текст и формат
            textBox.Text = "Sample Text Effect";
            
            // Получить формат текстового эффекта
            Shape shape = textBox;
            TextEffectFormat effectFormat = shape.TextEffect;
            
            // Установить свойства шрифта, включая FontSize
            effectFormat.FontName = "Arial";
            effectFormat.FontBold = true;
            effectFormat.FontItalic = false;
            effectFormat.FontSize = 18; // Demonstrating FontSize property
            
            // Сохраните книгу
            workbook.Save("TextEffectFontSizeDemo.xlsx");
            
            Console.WriteLine("Text effect with font size 18 created successfully.");
        }
    }
}
```

### См. также

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


