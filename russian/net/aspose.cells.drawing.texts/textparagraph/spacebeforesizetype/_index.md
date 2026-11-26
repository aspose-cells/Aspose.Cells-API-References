---
title: "TextParagraph.SpaceBeforeSizeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextParagraph. Получает и задает количество вертикального пробела, который будет присутствовать перед абзацем."
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/spacebeforesizetype/
---
## TextParagraph.SpaceBeforeSizeType property

Получает и задает количество вертикального пустого пространства, которое будет присутствовать перед абзацем.

```csharp
public LineSpaceSizeType SpaceBeforeSizeType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertySpaceBeforeSizeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте текстовое поле и получите его форму.
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Получите доступ ко второму абзацу.
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[1];
            
            // Установите свойства интервала абзаца.
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.SpaceBeforeSizeType = LineSpaceSizeType.Points;
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            
            paragraph.LineSpace = 12;
            paragraph.SpaceBefore = 8;
            paragraph.SpaceAfter = 10;
            
            // Сохраните и перезагрузите, чтобы продемонстрировать сохранность
            string outputPath = "TextParagraphSpacingDemo.xlsx";
            workbook.Save(outputPath);
            
            // Перезагрузить для проверки свойств
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
            
            Console.WriteLine("SpaceBeforeSizeType: " + loadedParagraph.SpaceBeforeSizeType);
            Console.WriteLine("SpaceBefore: " + loadedParagraph.SpaceBefore);
            Console.WriteLine("SpaceAfterSizeType: " + loadedParagraph.SpaceAfterSizeType);
            Console.WriteLine("SpaceAfter: " + loadedParagraph.SpaceAfter);
            Console.WriteLine("LineSpaceSizeType: " + loadedParagraph.LineSpaceSizeType);
            Console.WriteLine("LineSpace: " + loadedParagraph.LineSpace);
        }
    }
}
```

### См. также

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


