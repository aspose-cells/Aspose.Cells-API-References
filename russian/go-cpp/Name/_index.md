---
title: "Класс Name"
linktitle: "Name"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс Name. Инкапсулирует объект, представляющий name в Go."
type: docs
weight: 200
url: /ru/go-cpp/name/
---

## Name class

Представляет определённое имя для диапазона ячеек.

```go

type Name struct  {
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
| [GetComment](./getcomment/) | Получает и задает комментарий имени. Применяется только к Excel 2007 и более новым версиям. |
| [SetComment](./setcomment/) | Получает и задает комментарий имени. Применяется только к Excel 2007 и более новым версиям. |
| [GetText](./gettext/) | Получает текст имени объекта. |
| [SetText](./settext/) | Получает текст имени объекта. |
| [GetFullText](./getfulltext/) | Получает полный текст имени объекта с настройкой области. |
| [GetRefersTo](./getrefersto/) | Возвращает или задает формулу, к которой определено имя, начиная со знака равенства. |
| [SetRefersTo_String](./setrefersto_string/) | Возвращает или задает формулу, к которой определено имя, начиная со знака равенства. |
| [GetR1C1RefersTo](./getr1c1refersto/) | Получает или задает ссылку R1C1 имени. |
| [SetR1C1RefersTo](./setr1c1refersto/) | Получает или задает ссылку R1C1 имени. |
| [GetRefersTo_Bool_Bool](./getrefersto_bool_bool/) | Получить ссылку этого имени. |
| [GetRefersTo_Bool_Bool_Int_Int](./getrefersto_bool_bool_int_int/) | Получить ссылку этого имени, основанную на указанной ячейке. |
| [SetRefersTo_String_Bool_Bool](./setrefersto_string_bool_bool/) | Задать ссылку этого имени. |
| [IsReferred](./isreferred/) | Указывает, используется ли это имя в других формулах. |
| [IsVisible](./isvisible/) | Указывает, видимо ли имя. |
| [SetIsVisible](./setisvisible/) | Указывает, видимо ли имя. |
| [GetSheetIndex](./getsheetindex/) | Указывает, принадлежит ли это имя книге или листу. 0 = глобальное имя, иначе индекс листа (нумерация с 1). |
| [SetSheetIndex](./setsheetindex/) | Указывает, принадлежит ли это имя книге или листу. 0 = глобальное имя, иначе индекс листа (нумерация с 1). |
| [ToString](./tostring/) | Возвращает строку, представляющую текущий объект Range. |
| [GetRanges](./getranges/) | Получает все диапазоны, на которые ссылается это имя. |
| [GetRanges_Bool](./getranges_bool/) | Получает все диапазоны, на которые ссылается это имя. |
| [GetReferredAreas](./getreferredareas/) | Получает все ссылки, на которые ссылается это имя. |
| [GetRange](./getrange/) | Получает диапазон, если это имя ссылается на диапазон. |
| [GetRange_Bool](./getrange_bool/) | Получает диапазон, если это имя ссылается на диапазон |
| [GetRange_Int_Int_Int](./getrange_int_int_int/) | Получает диапазон, если это имя ссылается на диапазон. Если ссылка этого имени не абсолютна, диапазон может различаться для разных ячеек. |
