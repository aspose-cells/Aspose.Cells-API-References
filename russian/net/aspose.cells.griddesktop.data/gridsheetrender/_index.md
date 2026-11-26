---
title: "Класс GridSheetRender"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridDesktop.Data.GridSheetRender класс. Представляет рендер листа, который может отрисовывать лист в различные изображения, такие как BMP PNG JPEG TIFF. Конструктор этого класса должен использоваться после изменения стиля ячейки настройки страницы"
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridsheetrender/
---
## GridSheetRender class

Представляет рендер листа, который может выводить лист в различные изображения, такие как (BMP, PNG, JPEG, TIFF...). Конструктор этого класса должен использоваться после изменения параметров страницы и стиля ячеек.

```csharp
public class GridSheetRender
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridSheetRender](gridsheetrender/)(Worksheet, GridImageOrPrintOptions) | конструктор SheetRender, требуется лист и ImageOrPrintOptions в качестве параметров |

## Свойства

| Имя | Описание |
| --- | --- |
| [PageCount](../../aspose.cells.griddesktop.data/gridsheetrender/pagecount/) { get; } | Получает общее количество страниц текущего листа. |
| [PageScale](../../aspose.cells.griddesktop.data/gridsheetrender/pagescale/) { get; } | Получает рассчитанный масштаб страницы листа. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetPageSizeInch](../../aspose.cells.griddesktop.data/gridsheetrender/getpagesizeinch/)(int) | Получить размер страницы в дюймах выходного изображения. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage)(int) | Отрисовать определённую страницу в объект Bitmap. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_3)(int, Stream) | Отрисовать определённую страницу в поток. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_4)(int, string) | Отрисовать определённую страницу в файл. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Отрисовать определённую страницу в объект Graphics |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Отрисовать определённую страницу в объект Graphics |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter)(PrinterSettings) | Отрисовать лист на принтере |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_2)(string) | Отрисовать лист на принтере |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Отрисовать лист на принтере |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_3)(string, string) | Отрисовать лист на принтере |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff)(Stream) | Отрисовать весь лист как изображение Tiff в поток. |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff_1)(string) | Отрисовать весь лист как изображение Tiff в файл. |

### См. также

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


