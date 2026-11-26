---
title: "PageSetup.PrintQuality"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет качество печати"
type: docs
url: /ru/net/aspose.cells/pagesetup/printquality/
---
## PageSetup.PrintQuality property

Отображает качество печати.

```csharp
public int PrintQuality { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintQualityDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить качество печати 144 dpi
            worksheet.PageSetup.PrintQuality = 144;
            
            // Вывести текущую настройку качества печати
            Console.WriteLine("Print Quality: " + worksheet.PageSetup.PrintQuality);
            
            // Сохраните книгу
            workbook.Save("PrintQualityDemo.xls");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


