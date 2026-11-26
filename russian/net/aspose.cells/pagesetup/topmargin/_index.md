---
title: "PageSetup.TopMargin"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет размер верхнего поля в сантиметрах"
type: docs
url: /ru/net/aspose.cells/pagesetup/topmargin/
---
## PageSetup.TopMargin property

Отображает размер верхнего поля в сантиметрах.

```csharp
public double TopMargin { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyTopMarginDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            sheet.Cells["A1"].PutValue("Top Margin Demonstration");
            sheet.Cells["A2"].PutValue("This shows the effect of TopMargin property");

            // Установить свойства настройки страницы
            PageSetup pageSetup = sheet.PageSetup;
            pageSetup.TopMargin = 2.0; // 2 inches top margin
            pageSetup.LeftMargin = 0.5;
            pageSetup.RightMargin = 0.5;
            pageSetup.BottomMargin = 1.0;

            // Сохранить в PDF для демонстрации полей
            string outputPath = "TopMarginDemo.pdf";
            workbook.Save(outputPath, SaveFormat.Pdf);

            Console.WriteLine("Document with top margin of 2 inches saved to: " + outputPath);
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


