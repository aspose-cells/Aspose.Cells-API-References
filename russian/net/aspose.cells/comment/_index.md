---
title: "Класс Comment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Comment. Инкапсулирует объект, представляющий комментарий ячейки"
type: docs
url: /ru/net/aspose.cells/comment/
---
## Comment class

Инкапсулирует объект, представляющий комментарий ячейки.

```csharp
public class Comment
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Author](../../aspose.cells/comment/author/) { get; set; } | Получает и задает имя оригинального автора комментария |
| [AutoSize](../../aspose.cells/comment/autosize/) { get; set; } | Указывает, автоматически ли размер комментария регулируется в соответствии с его содержимым. Примечание: в некоторых особых случаях (например, в среде Mac) эта настройка может не сработать. Если настройка не сработает, замените её вызовом FitToTextSize(). |
| [Column](../../aspose.cells/comment/column/) { get; } | Получает индекс столбца комментария. |
| [CommentShape](../../aspose.cells/comment/commentshape/) { get; } | Получить объект Shape, представляющий форму, прикреплённую к указанному комментарию. |
| [Font](../../aspose.cells/comment/font/) { get; } | Получает шрифт комментария. |
| [Height](../../aspose.cells/comment/height/) { get; set; } | Представляет высоту комментария в пикселях. |
| [HeightCM](../../aspose.cells/comment/heightcm/) { get; set; } | Представляет высоту комментария в сантиметрах. |
| [HeightInch](../../aspose.cells/comment/heightinch/) { get; set; } | Представляет высоту комментария в дюймах. |
| [HtmlNote](../../aspose.cells/comment/htmlnote/) { get; set; } | Получает и задает HTML‑строку, содержащую данные и некоторые форматы в этом комментарии. |
| [IsThreadedComment](../../aspose.cells/comment/isthreadedcomment/) { get; } | Указывает, является ли этот комментарий ветвистым. |
| [IsVisible](../../aspose.cells/comment/isvisible/) { get; set; } | Указывает, видим ли комментарий. |
| [Note](../../aspose.cells/comment/note/) { get; set; } | Представляет содержание комментария. |
| [Row](../../aspose.cells/comment/row/) { get; } | Получает индекс строки комментария. |
| [TextHorizontalAlignment](../../aspose.cells/comment/texthorizontalalignment/) { get; set; } | Получает и задает тип горизонтального выравнивания текста в комментарии. |
| [TextOrientationType](../../aspose.cells/comment/textorientationtype/) { get; set; } | Получает и задает тип ориентации текста в комментарии. |
| [TextVerticalAlignment](../../aspose.cells/comment/textverticalalignment/) { get; set; } | Получает и задает тип вертикального выравнивания текста в комментарии. |
| [ThreadedComments](../../aspose.cells/comment/threadedcomments/) { get; } | Получает список ветвистых комментариев; |
| [Width](../../aspose.cells/comment/width/) { get; set; } | Представляет ширину комментария в пикселях. |
| [WidthCM](../../aspose.cells/comment/widthcm/) { get; set; } | Представляет ширину комментария в сантиметрах. |
| [WidthInch](../../aspose.cells/comment/widthinch/) { get; set; } | Представляет ширину комментария в дюймах. |

## Методы

| Имя | Описание |
| --- | --- |
| [Characters](../../aspose.cells/comment/characters/)(int, int) | Возвращает объект Characters, который представляет диапазон символов внутри текста комментария. |
| [FormatCharacters](../../aspose.cells/comment/formatcharacters/)(int, int, Font, StyleFlag) | Отформатировать некоторые символы с помощью настройки шрифта. |
| [GetRichFormattings](../../aspose.cells/comment/getrichformattings/)() | Возвращает все объекты Characters, которые представляют диапазон символов внутри текста комментария. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CommentDemo
    {
        public static void CommentExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            // Получить доступ к коллекции комментариев листа
            CommentCollection comments = worksheet.Comments;

            // Добавить комментарий к ячейке A1
            int commentIndex1 = comments.Add(0, 0);
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Font.Name = "Times New Roman";
            comment1.Font.Size = 12;
            comment1.Font.Color = System.Drawing.Color.Red;
            comment1.Author = "Carl.Yang";
            comment1.HtmlNote = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            comment1.IsVisible = true;
            comment1.TextOrientationType = TextOrientationType.TopToBottom;
            comment1.TextHorizontalAlignment = TextAlignmentType.Center;
            comment1.TextVerticalAlignment = TextAlignmentType.Center;
            comment1.AutoSize = true;
            comment1.HeightCM = 1.0;
            comment1.WidthCM = 1.0;
            comment1.Width = 10;
            comment1.Height = 10;
            comment1.WidthInch = 1.0;
            comment1.HeightInch = 1.0;

            // Получить доступ к форме комментария
            CommentShape shape = comment1.CommentShape;
            int w = shape.Width;
            int h = shape.Height;

            // Добавить комментарий в ячейку B2
            comments.Add("B2");
            Comment comment2 = comments["B2"];
            comment2.Note = "Second note.";

            // Сохраните книгу
            workbook.Save("CommentExample.xlsx");
            workbook.Save("CommentExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


