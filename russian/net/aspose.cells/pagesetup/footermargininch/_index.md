---
title: "PageSetup.FooterMarginInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет расстояние от нижнего края страницы до нижнего колонтитула в дюймах"
type: docs
url: /ru/net/aspose.cells/pagesetup/footermargininch/
---
## PageSetup.FooterMarginInch property

Представляет расстояние от нижнего края страницы до нижнего колонтитула, в дюймах.

```csharp
public double FooterMarginInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginInchDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к первому листу и его PageSetup
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Установите отступ нижнего колонтитула в дюймах
            pageSetup.FooterMarginInch = 0.5;
            
            // Установите другие отступы для демонстрации
            pageSetup.HeaderMarginInch = 0.3;
            pageSetup.TopMarginInch = 1.0;
            pageSetup.BottomMarginInch = 1.0;
            pageSetup.LeftMarginInch = 0.75;
            pageSetup.RightMarginInch = 0.75;
            
            // Сохраните книгу
            workbook.Save("PageSetupMargins.xlsx");
            
            // Вывести подтверждение
            Console.WriteLine("Footer margin set to: " + pageSetup.FooterMarginInch + " inches");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


