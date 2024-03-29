---
title: Comment
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует объект представляющий комментарий к ячейке.
type: docs
weight: 1080
url: /ru/net/aspose.cells/comment/
---
## Comment class

Инкапсулирует объект, представляющий комментарий к ячейке.

```csharp
public class Comment
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Author](../../aspose.cells/comment/author) { get; set; } | Получает и устанавливает имя исходного комментария author |
| [AutoSize](../../aspose.cells/comment/autosize) { get; set; } | Указывает, регулируется ли размер комментария автоматически в соответствии с его содержимым. |
| [Column](../../aspose.cells/comment/column) { get; } | Получает индекс столбца комментария. |
| [CommentShape](../../aspose.cells/comment/commentshape) { get; } | Получить объект Shape, представляющий фигуру, присоединенную к указанному комментарию. |
| [Font](../../aspose.cells/comment/font) { get; } | Получает шрифт комментария. |
| [Height](../../aspose.cells/comment/height) { get; set; } | Представляет высоту комментария в пикселях. |
| [HeightCM](../../aspose.cells/comment/heightcm) { get; set; } | Представляет высоту комментария в сантиметрах. |
| [HeightInch](../../aspose.cells/comment/heightinch) { get; set; } | Представляет высоту комментария в дюймах. |
| [HtmlNote](../../aspose.cells/comment/htmlnote) { get; set; } | Получает и задает строку html, содержащую данные и некоторые форматы в этом комментарии. |
| [IsThreadedComment](../../aspose.cells/comment/isthreadedcomment) { get; } | Указывает, является ли этот комментарий цепочкой комментариев. |
| [IsVisible](../../aspose.cells/comment/isvisible) { get; set; } | Указывает, виден комментарий или нет. |
| [Note](../../aspose.cells/comment/note) { get; set; } | Представляет содержимое комментария. |
| [Row](../../aspose.cells/comment/row) { get; } | Получает индекс строки комментария. |
| [TextHorizontalAlignment](../../aspose.cells/comment/texthorizontalalignment) { get; set; } | Получает и задает тип горизонтального выравнивания текста комментария. |
| [TextOrientationType](../../aspose.cells/comment/textorientationtype) { get; set; } | Получает и задает тип ориентации текста комментария. |
| [TextVerticalAlignment](../../aspose.cells/comment/textverticalalignment) { get; set; } | Получает и задает тип вертикального выравнивания текста комментария. |
| [ThreadedComments](../../aspose.cells/comment/threadedcomments) { get; } | Получает список цепочек комментариев; |
| [Width](../../aspose.cells/comment/width) { get; set; } | Представляет ширину комментария в пикселях. |
| [WidthCM](../../aspose.cells/comment/widthcm) { get; set; } | Представляет ширину комментария в сантиметрах. |
| [WidthInch](../../aspose.cells/comment/widthinch) { get; set; } | Представляет ширину комментария в дюймах. |

## Методы

| Имя | Описание |
| --- | --- |
| [Characters](../../aspose.cells/comment/characters)(int, int) | Возвращает объект символов, представляющий диапазон символов в тексте комментария. |
| [FormatCharacters](../../aspose.cells/comment/formatcharacters)(int, int, Font, StyleFlag) | Отформатируйте некоторые символы с помощью настройки шрифта. |
| [GetCharacters](../../aspose.cells/comment/getcharacters)() | Возвращает все объекты символов , представляющие диапазон символов в тексте комментария. |

### Примеры

```csharp
[C#]

Workbook workbook = new Workbook();
CommentCollection comments = workbook.Worksheets[0].Comments;

//Добавить комментарий к ячейке A1
int commentIndex1 = comments.Add(0, 0);
Comment comment1 = comments[commentIndex1];
comment1.Note = "First note.";
comment1.Font.Name = "Times New Roman";

//Добавить комментарий к ячейке B2
comments.Add("B2");
Comment comment2 = comments["B2"];
comment2.Note = "Second note.";

//делай свое дело

// Сохраняем файл excel.
workbook.Save("exmaple.xlsx");

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim comments as CommentCollection = workbook.Worksheets(0).Comments
 
'Добавить комментарий к ячейке A1
Dim commentIndex1 as Integer = comments.Add(0, 0)
Dim comment1 as Comment = comments(commentIndex1)
comment1.Note = "First note."
comment1.Font.Name = "Times New Roman"

'Добавить комментарий к ячейке B2
comments.Add("B2")
Dim comment2 As Comment = comments("B2")
comment2.Note = "Second note."
 
```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
