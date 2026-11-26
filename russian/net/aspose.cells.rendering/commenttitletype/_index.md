---
title: "Перечисление CommentTitleType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Rendering.CommentTitleType. Представляет тип заголовка комментария при рендеринге, когда комментарий установлен для отображения в конце листа"
type: docs
url: /ru/net/aspose.cells.rendering/commenttitletype/
---
## CommentTitleType enumeration

Представляет тип заголовка комментария при рендеринге, когда комментарий установлен для отображения в конце листа.

```csharp
public enum CommentTitleType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Cell | `0` | Представляет ячейку заголовка комментария. |
| Comment | `1` | Представляет комментарий заголовка комментария. |
| Note | `2` | Представляет заметку заголовка комментария. |
| Reply | `3` | Представляет ответ заголовка комментария. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCommentTitleTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создайте пользовательские настройки глобализации
                SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

                // Продемонстрируйте все значения перечисления CommentTitleType
                Console.WriteLine("Available CommentTitleType values:");
                Console.WriteLine($"Cell: {(int)CommentTitleType.Cell}");
                Console.WriteLine($"Comment: {(int)CommentTitleType.Comment}");
                Console.WriteLine($"Note: {(int)CommentTitleType.Note}");
                Console.WriteLine($"Reply: {(int)CommentTitleType.Reply}");

                // Установите пользовательские заголовки для каждого типа комментария
                globalizationSettings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // Примените настройки глобализации к рабочей книге
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Добавьте комментарий, чтобы продемонстрировать функциональность
                int commentIndex = worksheet.Comments.Add("A1");
                Comment comment = worksheet.Comments[commentIndex];
                comment.Note = "This is a test comment";
                comment.Author = "Test Author";

                // Сохраните книгу
                workbook.Save("CommentTitleTypeDemo.xlsx");

                Console.WriteLine("CommentTitleType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CommentTitleType demonstration: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


