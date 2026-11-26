---
title: "PageSetup.IsPercentScale"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Если это свойство равно False, свойства FitToPagesWide и FitToPagesTall управляют масштабированием листа"
type: docs
url: /ru/net/aspose.cells/pagesetup/ispercentscale/
---
## PageSetup.IsPercentScale property

Если это свойство равно False, свойства FitToPagesWide и FitToPagesTall управляют масштабированием листа.

```csharp
public bool IsPercentScale { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsPercentScaleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к PageSetup и установить масштабирование на 80% (процентный масштаб)
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.Zoom = 80;
            pageSetup.IsPercentScale = true;

            // Вывести настройки для демонстрации IsPercentScale
            Console.WriteLine("Zoom: " + pageSetup.Zoom);
            Console.WriteLine("IsPercentScale: " + pageSetup.IsPercentScale);

            // Сохраните книгу
            workbook.Save("PageSetup_IsPercentScale_Output.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


