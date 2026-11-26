---
title: "Range.ClearComments"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Очищает комментарии этого диапазона"
type: docs
url: /ru/net/aspose.cells/range/clearcomments/
---
## Range.ClearComments method

Очищает комментарии этого диапазона.

```csharp
public void ClearComments()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearCommentsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные и комментарии в ячейки
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A1"].PutValue("This is a comment on A1", true, false);
            worksheet.Cells["B2"].Value = "More Data";
            worksheet.Cells["B2"].PutValue("This is a comment on B2", true, false);

            try
            {
                // Создайте диапазон, включающий ячейки с комментариями
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // Очистить комментарии из диапазона
                range.ClearComments();

                Console.WriteLine("Comments cleared successfully from range A1:B2");
                Console.WriteLine($"Cell A1 value after clearing: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"Cell B2 value after clearing: {worksheet.Cells["B2"].Value}");

                // Сохраните книгу
                workbook.Save("ClearCommentsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ClearComments: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


