---
title: "Класс TextParagraphCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.Texts.TextParagraphCollection. Представляет все текстовые абзацы"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraphcollection/
---
## TextParagraphCollection class

Представляет все абзацы текста.

```csharp
public class TextParagraphCollection : IEnumerable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.cells.drawing.texts/textparagraphcollection/count/) { get; } | Получает количество текстовых абзацев. |
| [Item](../../aspose.cells.drawing.texts/textparagraphcollection/item/) { get; } | Получает объект [`TextParagraph`](../textparagraph/) по указанному индексу. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetEnumerator](../../aspose.cells.drawing.texts/textparagraphcollection/getenumerator/)() | Получает перечислитель абзацев. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextParagraphCollectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте текстовое поле на первый лист
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            
            // Установите многострочный текст
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Получите коллекцию абзацев
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Получите доступ и измените второй абзац
            TextParagraph secondParagraph = paragraphs[1];
            secondParagraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            secondParagraph.LineSpace = 20;
            secondParagraph.SpaceAfter = 30;
            secondParagraph.SpaceBefore = 40;
            
            // Сохраните книгу
            workbook.Save("TextParagraphCollectionDemo.xlsx");
            
            Console.WriteLine("Text paragraph formatting saved successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


