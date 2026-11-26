---
title: "GlobalizationSettings.GetCommentTitleName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает название заголовка комментария, зависящее от локали, в соответствии с типом заголовка комментария"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/getcommenttitlename/
---
## GlobalizationSettings.GetCommentTitleName method

Получает название заголовка комментария, зависящее от локали, в соответствии с типом заголовка комментария.

```csharp
public virtual string GetCommentTitleName(CommentTitleType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | CommentTitleType |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class GlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo : GlobalizationSettings
    {
        public override string GetCommentTitleName(CommentTitleType type)
        {
            switch (type)
            {
                case CommentTitleType.Cell:
                    return "Custom Cell Comment";
                case CommentTitleType.Reply:  // Changed from Threaded to Reply
                    return "Custom Threaded Comment";
                default:
                    return base.GetCommentTitleName(type);
            }
        }

        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new GlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo(); // Changed to use Settings

            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить тестовый комментарий
            int commentIndex = worksheet.Comments.Add("B5");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Test comment content";

            try
            {
                // Получить заголовок комментария для разных типов
                var cellTitle = workbook.Settings.GlobalizationSettings.GetCommentTitleName(CommentTitleType.Cell); // Changed to use Settings
                var threadedTitle = workbook.Settings.GlobalizationSettings.GetCommentTitleName(CommentTitleType.Reply); // Changed type and Settings

                Console.WriteLine($"Cell Comment Title: {cellTitle}");
                Console.WriteLine($"Threaded Comment Title: {threadedTitle}");

                // Установить автора комментария (заголовок), используя наши пользовательские настройки глобализации
                comment.Author = cellTitle; // Changed from Title to Author
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCommentTitleName method: {ex.Message}");
            }

            workbook.Save("GetCommentTitleNameDemo.xlsx");
        }
    }
}
```

### См. также

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


