---
title: "Класс SheetRender"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Rendering.SheetRender. Представляет рендер листа, который может выводить лист в различные изображения, такие как BMP, PNG, JPEG, TIFF. Конструктор этого класса должен использоваться после изменения стиля ячейки настройки страницы."
type: docs
url: /ru/net/aspose.cells.rendering/sheetrender/
---
## SheetRender class

Представляет рендер листа, который может выводить лист в различные изображения, такие как (BMP, PNG, JPEG, TIFF...). Конструктор этого класса должен использоваться после изменения параметров страницы и стиля ячеек.

```csharp
public class SheetRender
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SheetRender](sheetrender/)(Worksheet, ImageOrPrintOptions) | конструктор SheetRender, требуется лист и ImageOrPrintOptions в качестве параметров |

## Свойства

| Имя | Описание |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/sheetrender/pagecount/) { get; } | Получает общее количество страниц текущего листа. |
| [PageScale](../../aspose.cells.rendering/sheetrender/pagescale/) { get; } | Получает рассчитанный масштаб страницы листа. Возвращает установленный масштаб, если [`Zoom`](../../aspose.cells/pagesetup/zoom/) установлен. В противном случае возвращает рассчитанный масштаб согласно [`FitToPagesWide`](../../aspose.cells/pagesetup/fittopageswide/) и [`FitToPagesTall`](../../aspose.cells/pagesetup/fittopagestall/). |

## Методы

| Имя | Описание |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/sheetrender/customprint/)(bool, PrintPageEventArgs) | Клиент может управлять настройками страницы принтера при печати каждой страницы с помощью этой функции. |
| [Dispose](../../aspose.cells.rendering/sheetrender/dispose/)() | Освобождает ресурсы, созданные и используемые для рендеринга. |
| [GetPageSizeInch](../../aspose.cells.rendering/sheetrender/getpagesizeinch/)(int) | Получить размер страницы в дюймах выходного изображения. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage)(int) | Отрисовать определённую страницу в объект Bitmap. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_3)(int, Stream) | Отрисовать определённую страницу в поток. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_4)(int, string) | Отрисовать определённую страницу в файл. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Отрисовать определённую страницу в объект Graphics |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Отрисовать определённую страницу в объект Graphics |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter)(PrinterSettings) | Отрисовать лист на принтере |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_2)(string) | Отрисовать лист на принтере |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Отрисовать лист на принтере |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_4)(string, string) | Отрисовать лист на принтере |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_3)(string, int, int) | (**Obsolete.**) Отрисовать лист на принтере |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff)(Stream) | Отрисовать весь лист как изображение Tiff в поток. |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff_1)(string) | Отрисовать весь лист как изображение Tiff в файл. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassSheetRenderDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавьте примерные данные
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Настроить параметры страницы
            PageSetup pageSetup = sheet.PageSetup;
            pageSetup.PrintArea = "1:10";
            pageSetup.SetFitToPages(1, 1);

            // Создать SheetRender и продемонстрировать основную функциональность
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender sr = new SheetRender(sheet, options);
            
            Console.WriteLine($"Number of pages: {sr.PageCount}");
            Console.WriteLine($"Page scale: {sr.PageScale * 100}%");
            
            // Отрисовать первую страницу в изображение (демонстрация)
            sr.ToImage(0, "output_page1.png");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


