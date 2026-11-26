---
title: "TextParagraph.SpaceAfter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextParagraph. Получает и задает количество вертикального пустого пространства, которое будет присутствовать после абзаца"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/spaceafter/
---
## TextParagraph.SpaceAfter property

Получает и задает количество вертикального пустого пространства, которое будет присутствовать после абзаца.

```csharp
public double SpaceAfter { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertySpaceAfterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте текстовый блок и задайте текст
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Получите абзацы
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Настройте интервал второго абзаца
            TextParagraph p = paragraphs[1];
            p.LineSpaceSizeType = LineSpaceSizeType.Points;
            p.LineSpace = 2;
            p.SpaceAfter = 3; // Demonstrate SpaceAfter property
            p.SpaceBefore = 4;
            
            // Сохранить и проверить
            workbook.Save("TextParagraphPropertySpaceAfterDemo.xlsx");
            
            // Перезагрузите, чтобы проверить настройки
            Workbook loadedWorkbook = new Workbook("TextParagraphPropertySpaceAfterDemo.xlsx");
            TextParagraph loadedPara = loadedWorkbook.Worksheets[0].Shapes[0].TextBody.TextParagraphs[1];
            
            Console.WriteLine("SpaceAfter: " + loadedPara.SpaceAfter);
            Console.WriteLine("SpaceBefore: " + loadedPara.SpaceBefore);
            Console.WriteLine("LineSpace: " + loadedPara.LineSpace);
        }
    }
}
```

### См. также

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


