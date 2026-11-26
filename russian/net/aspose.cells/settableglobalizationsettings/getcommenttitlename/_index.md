---
title: "SettableGlobalizationSettings.GetCommentTitleName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Получает название заголовка комментария, зависящее от локали, в соответствии с типом заголовка комментария"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/getcommenttitlename/
---
## SettableGlobalizationSettings.GetCommentTitleName method

Получает название заголовка комментария, зависящее от локали, в соответствии с типом заголовка комментария.

```csharp
public override string GetCommentTitleName(CommentTitleType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | CommentTitleType | тип заголовка комментария |

### Возвращаемое значение

зависящее от локали название заголовка комментария

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SettableGlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать комментарий в ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";
            comment.IsVisible = true;

            // Создайте пользовательские настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Установить пользовательские названия заголовков комментариев для разных типов
            settings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
            settings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
            settings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
            settings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

            // Примените настройки глобализации к рабочей книге
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Получить и отобразить названия заголовков комментариев
                Console.WriteLine("Cell title: " + settings.GetCommentTitleName(CommentTitleType.Cell));
                Console.WriteLine("Comment title: " + settings.GetCommentTitleName(CommentTitleType.Comment));
                Console.WriteLine("Note title: " + settings.GetCommentTitleName(CommentTitleType.Note));
                Console.WriteLine("Reply title: " + settings.GetCommentTitleName(CommentTitleType.Reply));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCommentTitleName method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("CommentTitleNamesDemo.xlsx");
        }
    }
}
```

### См. также

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


