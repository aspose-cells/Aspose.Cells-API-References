---
title: "PageSetup.RightMarginInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет размер правого поля в дюймах"
type: docs
url: /ru/net/aspose.cells/pagesetup/rightmargininch/
---
## PageSetup.RightMarginInch property

Отображает размер правого поля в дюймах.

```csharp
public double RightMarginInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyRightMarginInchDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Получите доступ к PageSetup и установите RightMarginInch
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.RightMarginInch = 0.75; // Set right margin to 0.75 inches

            // Добавьте некоторые примерные данные, чтобы увидеть эффект
            worksheet.Cells["A1"].PutValue("Right Margin Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["B" + i].PutValue("Sample Data " + i);
            }

            // Сохраните книгу
            workbook.Save("RightMarginInchDemo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


