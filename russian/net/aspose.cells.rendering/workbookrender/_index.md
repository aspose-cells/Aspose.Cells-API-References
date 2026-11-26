---
title: "Класс WorkbookRender"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Rendering.WorkbookRender. Представляет рендеринг книги. Конструктор этого класса должен использоваться после изменения стиля ячейки настройки страницы"
type: docs
url: /ru/net/aspose.cells.rendering/workbookrender/
---
## WorkbookRender class

Представляет рендер книги. Конструктор этого класса должен использоваться после изменения параметров страницы и стиля ячеек.

```csharp
public class WorkbookRender
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WorkbookRender](workbookrender/)(Workbook, ImageOrPrintOptions) | Конструкция WorkbookRender |

## Свойства

| Имя | Описание |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/workbookrender/pagecount/) { get; } | Получает общее количество страниц книги. |

## Методы

| Имя | Описание |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/workbookrender/customprint/)(bool, PrintPageEventArgs) | Клиент может управлять настройками страницы принтера при печати каждой страницы с помощью этой функции. |
| [Dispose](../../aspose.cells.rendering/workbookrender/dispose/)() | Освобождает ресурсы, созданные и используемые для рендеринга. |
| [GetPageSizeInch](../../aspose.cells.rendering/workbookrender/getpagesizeinch/)(int) | Получить размер страницы в дюймах выходного изображения. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage)(int) | Отрисовать определённую страницу в объект Bitmap. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_3)(Stream) | Отрисовать всю книгу как изображение Tiff в поток. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_4)(string) | Отрисовать всю книгу как изображение Tiff в файл. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_1)(int, Stream) | Отрисовать определённую страницу в поток. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_2)(int, string) | Отрисовать определённую страницу в файл. |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter)(PrinterSettings) | Отрисовать книгу на принтере |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_2)(string) | Отрисовать книгу на принтере |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_1)(PrinterSettings, string) | Отрисовать книгу на принтере |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_4)(string, string) | Отрисовать книгу на принтере |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_3)(string, int, int) | (**Устарело.**) Отрисовать книгу на принтере |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassWorkbookRenderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные и задайте размер страницы
            worksheet.Cells["A1"].PutValue("Workbook Render Demo");
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            // Создать параметры изображения
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Создать рендеринг книги и получить размер страницы
            WorkbookRender render = new WorkbookRender(workbook, options);
            float[] pageSize = render.GetPageSizeInch(0);
            
            // Выведите результаты
            Console.WriteLine($"Page Width: {pageSize[0]} inches");
            Console.WriteLine($"Page Height: {pageSize[1]} inches");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


