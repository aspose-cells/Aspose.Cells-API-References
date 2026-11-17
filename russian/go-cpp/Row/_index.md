---
title: "Row Класс"
linktitle: "Row"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Row класс. Инкапсулирует объект, представляющий row в Go."
type: docs
weight: 200
url: /ru/go-cpp/row/
---

## Row class

Представляет одну строку в листе.

```go

type Row struct  {
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
| [GetCellByIndex](./getcellbyindex/) | Получить ячейку по конкретному индексу в коллекции ячеек этой строки. |
| [IsBlank](./isblank/) | Указывает, содержит ли строка какие-либо данные |
| [Get](./get/) | Получает ячейку. |
| [GetEnumerator](./getenumerator/) | Получает перечислитель ячеек |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Получает перечислитель, который перебирает ячейки в этой строке. |
| [GetCellOrNull](./getcellornull/) | Получает ячейку или null по конкретному индексу. |
| [IsCollapsed](./iscollapsed/) | является ли строка свернутой |
| [SetIsCollapsed](./setiscollapsed/) | является ли строка свернутой |
| [GetHeight](./getheight/) | Получает и задает высоту строки в единицах Points. |
| [SetHeight](./setheight/) | Получает и задает высоту строки в единицах Points. |
| [IsHidden](./ishidden/) | Указывает, скрыта ли строка. |
| [SetIsHidden](./setishidden/) | Указывает, скрыта ли строка. |
| [GetIndex](./getindex/) | Получает индекс этой строки. |
| [GetGroupLevel](./getgrouplevel/) | Получает уровень группы строки. |
| [SetGroupLevel](./setgrouplevel/) | Получает уровень группы строки. |
| [IsHeightMatched](./isheightmatched/) | Указывает, соответствует ли высота строки текущей настройке шрифта по умолчанию в рабочей книге. Значение true этого свойства также означает, что высота строки "автоматическая" без пользовательского значения высоты. |
| [SetIsHeightMatched](./setisheightmatched/) | Указывает, соответствует ли высота строки текущей настройке шрифта по умолчанию в рабочей книге. Значение true этого свойства также означает, что высота строки "автоматическая" без пользовательского значения высоты. |
| [GetStyle](./getstyle/) | Получает стиль этой строки. |
| [SetStyle](./setstyle/) | Устанавливает стиль этой строки. |
| [GetHasCustomStyle](./gethascustomstyle/) | Указывает, имеет ли эта строка пользовательские настройки стиля (отличные от стиля по умолчанию, наследуемого из рабочей книги). |
| [CopySettings](./copysettings/) | Копирует настройки строки, такие как стиль, высота, видимость и т.д. |
| [GetFirstCell](./getfirstcell/) | Получает первый объект ячейки в строке. |
| [GetFirstDataCell](./getfirstdatacell/) | Получает первую непустую ячейку в строке. |
| [GetLastCell](./getlastcell/) | Получает последний объект ячейки в строке. |
| [GetLastDataCell](./getlastdatacell/) | Получает последнюю непустую ячейку в строке. |
| [ApplyStyle](./applystyle/) | Применяет форматы ко всей строке. |
| [Equals_Object](./equals_object/) | Проверяет, ссылается ли этот объект на ту же строку, что и другой. |
| [Equals_Row](./equals_row/) | Проверяет, ссылается ли этот объект на ту же строку, что и другой объект строки. |
