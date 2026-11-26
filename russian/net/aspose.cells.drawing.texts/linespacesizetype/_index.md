---
title: "Перечисление LineSpaceSizeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.Texts.LineSpaceSizeType. Представляет тип единицы размера межстрочного интервала"
type: docs
url: /ru/net/aspose.cells.drawing.texts/linespacesizetype/
---
## LineSpaceSizeType enumeration

Представляет тип единицы размера межстрочного интервала.

```csharp
public enum LineSpaceSizeType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Percentage | `0` | Представляет в единице процента от размера текста. |
| Points | `1` | Представляет в единице точек. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassLineSpaceSizeTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить форму текстового поля
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Установить текстовое содержание
            textBox.Text = "Sample Text\nSecond Line";
            
            // Получить доступ к первому абзацу текстового поля
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];
            
            // Установить тип размера отступа после в точках
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            
            // Установить значение отступа после (12 точек)
            paragraph.SpaceAfter = 12;
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Text box with line spacing created successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


