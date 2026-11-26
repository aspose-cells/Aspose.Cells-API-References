---
title: "Comment.GetRichFormattings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Comment. Возвращает все объекты Characters, которые представляют диапазон символов в тексте комментария"
type: docs
url: /ru/net/aspose.cells/comment/getrichformattings/
---
## Comment.GetRichFormattings method

Возвращает все объекты Characters, которые представляют диапазон символов внутри текста комментария.

```csharp
public FontSetting[] GetRichFormattings()
```

### Возвращаемое значение

Все объекты Characters

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.HtmlNote = "<b>Bold</b>, <i>Italic</i>, <u>Underline</u>";

            // Получить форматирование богатого текста
            FontSetting[] formattings = comment.GetRichFormattings();

            // Отобразить информацию о форматировании
            Console.WriteLine("Rich Text Formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"StartIndex: {setting.StartIndex}, Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}, Italic: {setting.Font.IsItalic}, Underline: {setting.Font.Underline}");
            }
        }
    }
}
```

### См. также

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


