---
title: "Класс SheetRender"
linktitle: "SheetRender"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс SheetRender. Инкапсулирует объект, представляющий sheetrender в Go."
type: docs
weight: 200
url: /ru/go-cpp/sheetrender/
---

## SheetRender class

Представляет рендер листа, который может рендерить лист в различные изображения, такие как (BMP, PNG, JPEG, TIFF...). Конструктор этого класса должен использоваться после изменения параметров настройки страницы и стиля ячеек.

```go

type SheetRender struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewSheetRender](./newsheetrender/) | конструктор SheetRender, требует worksheet и ImageOrPrintOptions в качестве параметров |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetPageCount](./getpagecount/) | Получает общее количество страниц текущего листа. |
| [GetPageScale](./getpagescale/) | Получает вычисленный масштаб страницы листа. Возвращает установленный масштаб, если задан PageSetup.Zoom. В противном случае возвращает вычисленный масштаб в соответствии с PageSetup.FitToPagesWide и PageSetup.FitToPagesTall. |
| [GetPageSizeInch](./getpagesizeinch/) | Получить размер страницы в дюймах выходного изображения. |
| [ToImage_Int_String](./toimage_int_string/) | Отрисовать определённую страницу в файл. |
| [ToImage_Int](./toimage_int/) | Отрисовать определённую страницу в поток. |
| [ToTiff](./totiff/) | Рендерит весь лист как Tiff‑изображение в поток. |
| [ToTiff_String](./totiff_string/) | Рендерит весь лист как Tiff‑изображение в файл. |
| [Dispose](./dispose/) | Освобождает ресурсы, созданные и используемые для отрисовки. |
