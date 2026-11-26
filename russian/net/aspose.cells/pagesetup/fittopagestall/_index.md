---
title: "PageSetup.FitToPagesTall"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет количество страниц в высоту, до которого будет масштабироваться лист при печати. Значение по умолчанию — 1"
type: docs
url: /ru/net/aspose.cells/pagesetup/fittopagestall/
---
## PageSetup.FitToPagesTall property

Представляет количество страниц по высоте, до которого будет масштабироваться лист при печати. Значение по умолчанию — 1.

```csharp
public int FitToPagesTall { get; set; }
```

### Примечания

Вам нужно установить FitToPagesWide в ноль, если вы хотите разместить все строки на одной странице.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesTallDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные, чтобы лист охватывал несколько страниц
            for (int i = 0; i < 100; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
                }
            }

            // Получить объект PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Установить область печати
            pageSetup.PrintArea = "A1:J100";
            
            // Установить свойство FitToPagesTall, чтобы разместить все строки на одной странице
            pageSetup.FitToPagesTall = 1;
            
            // Установить свойство FitToPagesWide, чтобы разместить все столбцы на одной странице
            pageSetup.FitToPagesWide = 1;
            
            // Установить размер бумаги
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // Печатать линии сетки
            pageSetup.PrintGridlines = true;

            // Создать параметры рендеринга
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Создать рендерер листа
            SheetRender render = new SheetRender(worksheet, options);
            
            // Вывести масштаб страницы
            Console.WriteLine($"Page scale: {Math.Round(render.PageScale, 2)}");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


