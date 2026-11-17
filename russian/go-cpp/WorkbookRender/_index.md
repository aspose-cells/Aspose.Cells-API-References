---
title: "WorkbookRender Класс"
linktitle: "WorkbookRender"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "WorkbookRender класс. Инкапсулирует объект, представляющий workbookrender в Go."
type: docs
weight: 200
url: /ru/go-cpp/workbookrender/
---

## WorkbookRender class

Представляет рендер книги. Конструктор этого класса должен использоваться после изменения параметров настройки страницы и стиля ячеек.

```go

type WorkbookRender struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewWorkbookRender](./newworkbookrender/) | Конструктор WorkbookRender |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetPageCount](./getpagecount/) | Получает общее количество страниц рабочей книги. |
| [GetPageSizeInch](./getpagesizeinch/) | Получить размер страницы в дюймах выходного изображения. |
| [ToImage](./toimage/) | Отрисовать всю рабочую книгу как Tiff-изображение в поток. |
| [ToImage_String](./toimage_string/) | Отрисовать всю рабочую книгу как Tiff-изображение в файл. |
| [ToImage_Int_String](./toimage_int_string/) | Отрисовать определённую страницу в файл. |
| [ToImage_Int](./toimage_int/) | Отрисовать определённую страницу в поток. |
| [Dispose](./dispose/) | Освобождает ресурсы, созданные и используемые для отрисовки. |
