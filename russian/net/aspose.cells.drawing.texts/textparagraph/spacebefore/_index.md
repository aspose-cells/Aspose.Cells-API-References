---
title: "TextParagraph.SpaceBefore"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextParagraph. Получает и задает количество вертикального пробела, который будет присутствовать перед абзацем."
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/spacebefore/
---
## TextParagraph.SpaceBefore property

Получает и задает количество вертикального пустого пространства, которое будет присутствовать перед абзацем.

```csharp
public double SpaceBefore { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertySpaceBeforeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте текстовый блок и задайте текст
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Получите абзацы
            Aspose.Cells.Drawing.Texts.TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Настройте интервал второго абзаца
            Aspose.Cells.Drawing.Texts.TextParagraph p = paragraphs[1];
            p.LineSpaceSizeType = Aspose.Cells.Drawing.Texts.LineSpaceSizeType.Points;
            p.LineSpace = 2;
            p.SpaceAfter = 3;
            p.SpaceBefore = 4; // Demonstrate SpaceBefore property
            
            // Сохранить и проверить
            string outputPath = "output_SpaceBeforeDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Demo completed. File saved: " + outputPath);
        }
    }
}
```

### См. также

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


