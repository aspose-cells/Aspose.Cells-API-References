---
title: "PageSetup.LeftMarginInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет размер левого отступа в дюймах."
type: docs
url: /ru/net/aspose.cells/pagesetup/leftmargininch/
---
## PageSetup.LeftMarginInch property

Представляет размер левого поля, в дюймах.

```csharp
public double LeftMarginInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyLeftMarginInchDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Доступ к PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Установите левый отступ в дюймах (0,39 дюйма ≈ 1 см)
            pageSetup.LeftMarginInch = 0.39;

            // Добавьте некоторые данные, чтобы продемонстрировать отступ
            worksheet.Cells["A1"].PutValue("Left Margin Demonstration");
            worksheet.Cells["A2"].PutValue("Left margin set to 0.39 inches");

            // Сохраните книгу
            workbook.Save("LeftMarginInchDemo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


