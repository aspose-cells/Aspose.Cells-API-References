---
title: "MsoFillFormat.Transparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFillFormat. Возвращает или задает степень прозрачности указанной заливки в виде значения от 0.0 (непрозрачный) до 1.0 (полностью прозрачный)"
type: docs
url: /ru/net/aspose.cells.drawing/msofillformat/transparency/
---
## MsoFillFormat.Transparency property

Возвращает или задает степень прозрачности указанного заполнения в виде значения от 0.0 (непрозрачный) до 1.0 (прозрачный).

```csharp
public double Transparency { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Установить свойства формата заливки, включая прозрачность
            comment.CommentShape.FillFormat.IsVisible = true;
            comment.CommentShape.FillFormat.ForeColor = System.Drawing.Color.Red;
            comment.CommentShape.FillFormat.BackColor = System.Drawing.Color.Yellow;
            
            // Установить прозрачность (0.0 = полностью непрозрачно, 1.0 = полностью прозрачно)
            comment.CommentShape.FillFormat.Transparency = 0.5;

            // Сохраните книгу
            workbook.Save("CommentTransparencyDemo.xlsx");

            // Загрузить сохранённую книгу, чтобы проверить прозрачность
            Workbook verifyWorkbook = new Workbook("CommentTransparencyDemo.xlsx");
            Comment verifyComment = verifyWorkbook.Worksheets[0].Comments[0];
            
            // Вывести значение прозрачности, чтобы продемонстрировать, что оно было сохранено и загружено корректно
            Console.WriteLine("Comment fill transparency: " + 
                verifyComment.CommentShape.FillFormat.Transparency);
        }
    }
}
```

### См. также

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


