---
title: "PageSetup.FirstPageNumber"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет номер первой страницы, который будет использоваться при печати этого листа"
type: docs
url: /ru/net/aspose.cells/pagesetup/firstpagenumber/
---
## PageSetup.FirstPageNumber property

Определяет номер первой страницы, который будет использоваться при печати этого листа.

```csharp
public int FirstPageNumber { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFirstPageNumberDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить свойства настройки страницы
            worksheet.PageSetup.IsAutoFirstPageNumber = false;
            worksheet.PageSetup.FirstPageNumber = 3;
            
            // Печать результатов
            Console.WriteLine("IsAutoFirstPageNumber: " + worksheet.PageSetup.IsAutoFirstPageNumber);
            Console.WriteLine("FirstPageNumber: " + worksheet.PageSetup.FirstPageNumber);
            
            // Сохраните книгу
            workbook.Save("PageSetupFirstPageNumberDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


