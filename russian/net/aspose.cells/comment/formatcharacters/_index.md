---
title: "Comment.FormatCharacters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Comment. Форматирует некоторые символы с настройкой шрифта"
type: docs
url: /ru/net/aspose.cells/comment/formatcharacters/
---
## Comment.FormatCharacters method

Отформатировать некоторые символы с помощью настройки шрифта.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | Int32 | Начальный индекс. |
| длина | Int32 | Длина. |
| шрифт | Шрифт | Настройка шрифта. |
| флаг | StyleFlag | Флаг настройки шрифта. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CommentMethodFormatCharactersWithInt32Int32FontStyleFlagDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentRow = 0;
            int commentColumn = 0;
            Comment comment = worksheet.Comments[commentRow, commentColumn];
            comment.Note = "This is a sample comment with formatted text.";

            // Создать шрифт для форматирования — необходимо получить его из стиля рабочей книги
            Aspose.Cells.Font font = workbook.CreateStyle().Font;
            font.IsBold = true;
            font.Color = Color.Red;
            font.Size = 14;
            font.Underline = FontUnderlineType.Single;

            // Создать флаг стиля, чтобы указать, какие свойства шрифта применять
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontBold = true;
            styleFlag.FontColor = true;
            styleFlag.FontSize = true;
            styleFlag.FontUnderline = true;

            try
            {
                // Форматировать символы, начиная с индекса 5, длиной 10
                comment.FormatCharacters(5, 10, font, styleFlag);

                Console.WriteLine("FormatCharacters method executed successfully on the comment.");
                
                // Сделать комментарий видимым, чтобы увидеть эффект
                comment.IsVisible = true;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FormatCharacters method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("CommentFormatCharactersDemo.xlsx");
        }
    }
}
```

### См. также

* class [Font](../../font/)
* class [StyleFlag](../../styleflag/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


