---
title: "Класс TextParagraph"
linktitle: "TextParagraph"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс TextParagraph. Инкапсулирует объект, представляющий текстовый абзац в Go."
type: docs
weight: 200
url: /ru/go-cpp/textparagraph/
---

## TextParagraph class

Представляет настройку абзаца текста.

```go

type TextParagraph struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewTextParagraph](./newtextparagraph/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetBullet](./getbullet/) | Получает маркер. |
| [GetType](./gettype/) | Получает тип текстового узла. |
| [GetLineSpaceSizeType](./getlinespacesizetype/) | Получает и задает количество вертикального пробела, которое будет использоваться внутри абзаца. |
| [SetLineSpaceSizeType](./setlinespacesizetype/) | Получает и задает количество вертикального пробела, которое будет использоваться внутри абзаца. |
| [GetLineSpace](./getlinespace/) | Получает и задает количество вертикального пробела, которое будет использоваться внутри абзаца. |
| [SetLineSpace](./setlinespace/) | Получает и задает количество вертикального пробела, которое будет использоваться внутри абзаца. |
| [GetSpaceAfterSizeType](./getspaceaftersizetype/) | Получает и задает количество вертикального пробела, которое будет присутствовать после абзаца. |
| [SetSpaceAfterSizeType](./setspaceaftersizetype/) | Получает и задает количество вертикального пробела, которое будет присутствовать после абзаца. |
| [GetSpaceAfter](./getspaceafter/) | Получает и задает количество вертикального пробела, которое будет присутствовать после абзаца. |
| [SetSpaceAfter](./setspaceafter/) | Получает и задает количество вертикального пробела, которое будет присутствовать после абзаца. |
| [GetSpaceBeforeSizeType](./getspacebeforesizetype/) | Получает и задает количество вертикального пробела, которое будет присутствовать перед абзацем. |
| [SetSpaceBeforeSizeType](./setspacebeforesizetype/) | Получает и задает количество вертикального пробела, которое будет присутствовать перед абзацем. |
| [GetSpaceBefore](./getspacebefore/) | Получает и задает количество вертикального пробела, которое будет присутствовать перед абзацем. |
| [SetSpaceBefore](./setspacebefore/) | Получает и задает количество вертикального пробела, которое будет присутствовать перед абзацем. |
| [GetStops](./getstops/) | Получает список табуляций. |
| [IsLatinLineBreak](./islatinlinebreak/) | Указывает, может ли латинское слово быть разбито пополам и перенесено на следующую строку без добавления дефиса. |
| [SetIsLatinLineBreak](./setislatinlinebreak/) | Указывает, может ли латинское слово быть разбито пополам и перенесено на следующую строку без добавления дефиса. |
| [IsEastAsianLineBreak](./iseastasianlinebreak/) | Указывает, может ли слово восточноазиатского языка быть разбито пополам и перенесено на следующую строку без добавления дефиса. |
| [SetIsEastAsianLineBreak](./setiseastasianlinebreak/) | Указывает, может ли слово восточноазиатского языка быть разбито пополам и перенесено на следующую строку без добавления дефиса. |
| [IsHangingPunctuation](./ishangingpunctuation/) | Указывает, должна ли пунктуация принудительно размещаться в строке текста или переноситься на другую строку. |
| [SetIsHangingPunctuation](./setishangingpunctuation/) | Указывает, должна ли пунктуация принудительно размещаться в строке текста или переноситься на другую строку. |
| [GetRightMargin](./getrightmargin/) | Указывает правый отступ абзаца. |
| [SetRightMargin](./setrightmargin/) | Указывает правый отступ абзаца. |
| [GetLeftMargin](./getleftmargin/) | Указывает левый отступ абзаца. |
| [SetLeftMargin](./setleftmargin/) | Указывает левый отступ абзаца. |
| [GetFirstLineIndent](./getfirstlineindent/) | Указывает размер отступа, который будет применён к первой строке текста в абзаце. |
| [SetFirstLineIndent](./setfirstlineindent/) | Указывает размер отступа, который будет применён к первой строке текста в абзаце. |
| [GetFontAlignType](./getfontaligntype/) | Определяет, где вертикально на строке текста находятся фактические слова. Это касается вертикального размещения символов относительно базовых линий. |
| [SetFontAlignType](./setfontaligntype/) | Определяет, где вертикально на строке текста находятся фактические слова. Это касается вертикального размещения символов относительно базовых линий. |
| [GetAlignmentType](./getalignmenttype/) | Получает и задаёт тип горизонтального выравнивания текста абзаца. |
| [SetAlignmentType](./setalignmenttype/) | Получает и задаёт тип горизонтального выравнивания текста абзаца. |
| [GetDefaultTabSize](./getdefaulttabsize/) | Получает и задаёт размер по умолчанию для символа табуляции в этом абзаце. |
| [SetDefaultTabSize](./setdefaulttabsize/) | Получает и задаёт размер по умолчанию для символа табуляции в этом абзаце. |
| [GetChildren](./getchildren/) | Получает все текстовые фрагменты в этом абзаце. Если абзац пуст, возвращает сам абзац. |
| [GetStartIndex](./getstartindex/) | Получает начальный индекс символов. |
| [GetLength](./getlength/) | Получает длину символов. |
| [GetFont](./getfont/) | Возвращает шрифт этого объекта. |
| [SetWordArtStyle](./setwordartstyle/) | Устанавливает предустановленный стиль WordArt. |
| [GetTextOptions](./gettextoptions/) | Возвращает параметры текста. |
