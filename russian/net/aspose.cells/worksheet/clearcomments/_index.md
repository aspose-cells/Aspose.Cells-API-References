---
title: "Worksheet.ClearComments"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Очищает все комментарии в проектируемой таблице"
type: docs
url: /ru/net/aspose.cells/worksheet/clearcomments/
---
## Worksheet.ClearComments method

Очищает все комментарии в проектируемой таблице.

```csharp
public void ClearComments()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodClearCommentsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные комментарии в ячейки, используя ссылки на ячейки
            int comment1 = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1].Note = "This is comment 1";
            
            int comment2 = worksheet.Comments.Add("B3");
            worksheet.Comments[comment2].Note = "This is comment 2";
            
            int comment3 = worksheet.Comments.Add("C5");
            worksheet.Comments[comment3].Note = "This is comment 3";

            // Показать количество комментариев до очистки
            Console.WriteLine($"Comments count before ClearComments(): {worksheet.Comments.Count}");

            // Очистить все комментарии с листа
            worksheet.ClearComments();

            // Показать количество комментариев после очистки
            Console.WriteLine($"Comments count after ClearComments(): {worksheet.Comments.Count}");

            // Сохраните книгу
            workbook.Save("ClearCommentsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


