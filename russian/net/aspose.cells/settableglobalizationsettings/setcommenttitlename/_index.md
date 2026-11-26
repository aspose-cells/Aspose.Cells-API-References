---
title: "SettableGlobalizationSettings.SetCommentTitleName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Получает название заголовка комментария, зависящее от локали, в соответствии с типом заголовка комментария"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/setcommenttitlename/
---
## SettableGlobalizationSettings.SetCommentTitleName method

Получает название заголовка комментария, зависящее от локали, в соответствии с типом заголовка комментария.

```csharp
public void SetCommentTitleName(CommentTitleType type, string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | CommentTitleType | тип заголовка комментария |
| name | String | зависящее от локали название заголовка комментария |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SettableGlobalizationSettingsMethodSetCommentTitleNameWithCommentTitleTypeStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            comment.IsVisible = true;

            // Создать настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Установить пользовательские названия заголовков комментариев для разных типов
                settings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                settings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                settings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                settings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // Примените настройки глобализации к рабочей книге
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetCommentTitleName method executed successfully with parameters (CommentTitleType, String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCommentTitleName method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("MethodSetCommentTitleNameDemo.xlsx");
        }
    }
}
```

### См. также

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


