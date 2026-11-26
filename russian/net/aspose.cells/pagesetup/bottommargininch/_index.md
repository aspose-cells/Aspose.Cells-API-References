---
title: "PageSetup.BottomMarginInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет размер нижнего поля в дюймах"
type: docs
url: /ru/net/aspose.cells/pagesetup/bottommargininch/
---
## PageSetup.BottomMarginInch property

Определяет размер нижнего поля в дюймах.

```csharp
public double BottomMarginInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBottomMarginInchDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Обратиться к PageSetup первого листа
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // Установить различные поля в дюймах
            setup.HeaderMarginInch = 0.1;
            setup.FooterMarginInch = 0.2;
            setup.TopMarginInch = 0.3;
            setup.BottomMarginInch = 0.4; // Demonstrating BottomMarginInch property
            setup.LeftMarginInch = 0.5;
            setup.RightMarginInch = 0.6;
            
            // Сохраните книгу
            workbook.Save("PageMarginsDemo.xlsx");
            
            // Отобразить подтверждение
            Console.WriteLine("Workbook saved with bottom margin set to: " + setup.BottomMarginInch + " inches");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


