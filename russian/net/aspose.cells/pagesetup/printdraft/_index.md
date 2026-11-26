---
title: "PageSetup.PrintDraft"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет, будет ли лист печататься без графики"
type: docs
url: /ru/net/aspose.cells/pagesetup/printdraft/
---
## PageSetup.PrintDraft property

Представляет, будет ли лист печататься без графики.

```csharp
public bool PrintDraft { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintDraftDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Доступ к объекту PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Установите свойство PrintDraft в true
            pageSetup.PrintDraft = true;
            Console.WriteLine("PrintDraft set to: " + pageSetup.PrintDraft);

            // Измените свойство PrintDraft на false
            pageSetup.PrintDraft = false;
            Console.WriteLine("PrintDraft changed to: " + pageSetup.PrintDraft);

            // Сохраните книгу
            workbook.Save("PageSetup_PrintDraft_Example.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


