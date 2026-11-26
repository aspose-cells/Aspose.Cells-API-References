---
title: "PageSetup.HeaderMarginInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет расстояние от верхней части страницы до заголовка в дюймах"
type: docs
url: /ru/net/aspose.cells/pagesetup/headermargininch/
---
## PageSetup.HeaderMarginInch property

Представляет расстояние от верхнего края страницы до верхнего колонтитула, в дюймах.

```csharp
public double HeaderMarginInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyHeaderMarginInchDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу и его PageSetup
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Установить отступ заголовка в дюймах
            pageSetup.HeaderMarginInch = 0.5;
            
            // Установите другие отступы для демонстрации
            pageSetup.FooterMarginInch = 0.25;
            pageSetup.TopMarginInch = 1.0;
            pageSetup.BottomMarginInch = 1.0;
            pageSetup.LeftMarginInch = 0.75;
            pageSetup.RightMarginInch = 0.75;

            // Сохраните книгу
            workbook.Save("PageSetupMargins.xlsx");

            // Отобразить значение отступа заголовка
            Console.WriteLine("Header Margin (inches): " + pageSetup.HeaderMarginInch);
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


