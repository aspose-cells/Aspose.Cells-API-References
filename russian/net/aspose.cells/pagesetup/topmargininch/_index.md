---
title: "PageSetup.TopMarginInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет размер верхнего поля в дюймах"
type: docs
url: /ru/net/aspose.cells/pagesetup/topmargininch/
---
## PageSetup.TopMarginInch property

Отображает размер верхнего поля в дюймах.

```csharp
public double TopMarginInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyTopMarginInchDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Установить верхнее поле в 1,5 дюйма
            sheet.PageSetup.TopMarginInch = 1.5;

            // Получить и вывести значение верхнего поля
            Console.WriteLine("Top Margin (inches): " + sheet.PageSetup.TopMarginInch);

            // Сохраните книгу
            workbook.Save("PageSetup_TopMarginInch_Example.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


