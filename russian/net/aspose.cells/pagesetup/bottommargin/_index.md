---
title: "PageSetup.BottomMargin"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет размер нижнего поля в сантиметрах"
type: docs
url: /ru/net/aspose.cells/pagesetup/bottommargin/
---
## PageSetup.BottomMargin property

Определяет размер нижнего поля в сантиметрах.

```csharp
public double BottomMargin { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBottomMarginDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите некоторые примерные данные
            worksheet.Cells["A1"].PutValue("Sample Text for Margin Demonstration");
            
            // Настройте параметры страницы с помощью BottomMargin
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.BottomMargin = 0.5; // 0.5 inch bottom margin
            pageSetup.TopMargin = 1.0;    // 1 inch top margin
            pageSetup.LeftMargin = 0.75;  // 0.75 inch left margin
            pageSetup.RightMargin = 0.75; // 0.75 inch right margin

            // Сохраните в PDF, чтобы продемонстрировать поля
            workbook.Save("PageMarginsDemo.pdf", SaveFormat.Pdf);

            Console.WriteLine("Document with bottom margin of 0.5 inches created successfully.");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


