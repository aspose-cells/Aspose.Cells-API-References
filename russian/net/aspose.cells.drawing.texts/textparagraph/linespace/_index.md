---
title: "TextParagraph.LineSpace"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextParagraph. Получает и задает количество вертикального пробела, который будет использоваться внутри абзаца"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/linespace/
---
## TextParagraph.LineSpace property

Получает и задает количество вертикального пустого пространства, которое будет использоваться в абзаце.

```csharp
public double LineSpace { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyLineSpaceDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить форму текстового поля
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First line\nSecond line";
            
            // Получить доступ к текстовым абзацам
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Настройте межстрочный интервал для второго абзаца
            TextParagraph paragraph = paragraphs[1];
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.LineSpace = 2; // Set line spacing to 2 points
            
            // Сохраните и перезагрузите, чтобы продемонстрировать сохранность
            string outputPath = "output_LineSpaceDemo.xlsx";
            workbook.Save(outputPath);
            
            // Перезагрузите, чтобы проверить настройки
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
            
            Console.WriteLine("Line space: " + loadedParagraph.LineSpace);
            Console.WriteLine("Line space type: " + loadedParagraph.LineSpaceSizeType);
        }
    }
}
```

### См. также

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


