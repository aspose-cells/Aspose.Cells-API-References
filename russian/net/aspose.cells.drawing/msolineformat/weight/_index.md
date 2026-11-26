---
title: "MsoLineFormat.Weight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoLineFormat. Возвращает или задаёт толщину линии в единицах pt"
type: docs
url: /ru/net/aspose.cells.drawing/msolineformat/weight/
---
## MsoLineFormat.Weight property

Возвращает или задает толщину линии в единицах pt.

```csharp
public double Weight { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyWeightDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Установить текст комментария
            comment.Note = "Sample comment";
            
            // Получить доступ к формату линии формы комментария и установить толщину
            comment.CommentShape.LineFormat.Weight = 0.75;
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Проверить, что толщина была установлена правильно
            Console.WriteLine("Line weight: " + worksheet.Comments[0].CommentShape.LineFormat.Weight);
        }
    }
}
```

### См. также

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


