---
title: "PageSetup.PaperSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет размер бумаги"
type: docs
url: /ru/net/aspose.cells/pagesetup/papersize/
---
## PageSetup.PaperSize property

Представляет размер бумаги.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Установить размер бумаги на Envelope B6
            sheet.PageSetup.PaperSize = PaperSizeType.PaperEnvelopeB6;

            // Печать текущего размера бумаги
            Console.WriteLine("Current paper size: " + sheet.PageSetup.PaperSize);

            // Сохраните книгу
            workbook.Save("PageSetup_PaperSizeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PaperSizeType](../../papersizetype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


