---
title: "Класс Comment"
linktitle: "Comment"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс Comment. Инкапсулирует объект, представляющий комментарий в Go."
type: docs
weight: 200
url: /ru/go-cpp/comment/
---

## Comment class

Инкапсулирует объект, представляющий комментарий ячейки.

```go

type Comment struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetAuthor](./getauthor/) | Получает и задает Name оригинального автора комментария |
| [SetAuthor](./setauthor/) | Получает и задает Name оригинального автора комментария |
| [GetCommentShape](./getcommentshape/) | Получить объект Shape, который представляет форму, прикреплённую к указанному комментарию. |
| [GetRow](./getrow/) | Получает индекс строки комментария. |
| [GetColumn](./getcolumn/) | Получает индекс столбца комментария. |
| [IsThreadedComment](./isthreadedcomment/) | Указывает, является ли этот комментарий ветвистым. |
| [GetThreadedComments](./getthreadedcomments/) | Получает список ветвистых комментариев; |
| [GetNote](./getnote/) | Представляет содержание комментария. |
| [SetNote](./setnote/) | Представляет содержание комментария. |
| [GetHtmlNote](./gethtmlnote/) | Получает и задает строку html, содержащую данные и некоторые форматы в этом комментарии. |
| [SetHtmlNote](./sethtmlnote/) | Получает и задает строку html, содержащую данные и некоторые форматы в этом комментарии. |
| [GetFont](./getfont/) | Получает шрифт комментария. |
| [FormatCharacters](./formatcharacters/) | Форматировать некоторые символы с помощью настройки шрифта. |
| [Characters](./characters/) | Возвращает объект Characters, представляющий диапазон символов в тексте комментария. |
| [GetRichFormattings](./getrichformattings/) | Возвращает все объекты Characters, представляющие диапазон символов в тексте комментария. |
| [IsVisible](./isvisible/) | Представляет, видим ли комментарий или нет. |
| [SetIsVisible](./setisvisible/) | Представляет, видим ли комментарий или нет. |
| [GetTextOrientationType](./gettextorientationtype/) | Получает и задает тип ориентации текста комментария. |
| [SetTextOrientationType](./settextorientationtype/) | Получает и задает тип ориентации текста комментария. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Получает и задает тип горизонтального выравнивания текста комментария. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Получает и задает тип горизонтального выравнивания текста комментария. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Получает и задает тип вертикального выравнивания текста комментария. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Получает и задает тип вертикального выравнивания текста комментария. |
| [GetAutoSize](./getautosize/) | Указывает, автоматически ли размер комментария регулируется в соответствии с его содержимым. Примечание: в некоторых особых случаях (например, в среде Mac) эта настройка может не сработать. Если настройка не сработает, пожалуйста, замените её на FitToTextSize(). |
| [SetAutoSize](./setautosize/) | Указывает, автоматически ли размер комментария регулируется в соответствии с его содержимым. Примечание: в некоторых особых случаях (например, в среде Mac) эта настройка может не сработать. Если настройка не сработает, пожалуйста, замените её на FitToTextSize(). |
| [GetHeightCM](./getheightcm/) | Представляет высоту комментария в сантиметрах. |
| [SetHeightCM](./setheightcm/) | Представляет высоту комментария в сантиметрах. |
| [GetWidthCM](./getwidthcm/) | Представляет ширину комментария в сантиметрах. |
| [SetWidthCM](./setwidthcm/) | Представляет ширину комментария в сантиметрах. |
| [GetWidth](./getwidth/) | Представляет ширину комментария в пикселях. |
| [SetWidth](./setwidth/) | Представляет ширину комментария в пикселях. |
| [GetHeight](./getheight/) | Представляет высоту комментария в пикселях. |
| [SetHeight](./setheight/) | Представляет высоту комментария в пикселях. |
| [GetWidthInch](./getwidthinch/) | Представляет ширину комментария в дюймах. |
| [SetWidthInch](./setwidthinch/) | Представляет ширину комментария в дюймах. |
| [GetHeightInch](./getheightinch/) | Представляет высоту комментария в дюймах. |
| [SetHeightInch](./setheightinch/) | Представляет высоту комментария в дюймах. |
