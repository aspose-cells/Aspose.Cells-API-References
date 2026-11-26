---
title: "TextParagraph.LineSpaceSizeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextParagraph. Получает и задает количество вертикального пробела, который будет использоваться внутри абзаца"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/linespacesizetype/
---
## TextParagraph.LineSpaceSizeType property

Получает и задает количество вертикального пустого пространства, которое будет использоваться в абзаце.

```csharp
public LineSpaceSizeType LineSpaceSizeType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyLineSpaceSizeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте текстовое поле и задайте текст
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First line\nSecond line";
            
            // Получите второй абзац
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[1];
            
            // Задать свойства межстрочного интервала
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.LineSpace = 2;
            paragraph.SpaceAfter = 3;
            paragraph.SpaceBefore = 4;
            
            // Сохраните и выведите
            workbook.Save("TextParagraphPropertyLineSpaceSizeTypeDemo_output.xlsx");
            
            Console.WriteLine("Demo executed successfully. Output file created.");
        }
    }
}
```

### См. также

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


