---
title: "PageSetup.PrintCopies"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Получает и задает количество копий для печати"
type: docs
url: /ru/net/aspose.cells/pagesetup/printcopies/
---
## PageSetup.PrintCopies property

Получает и задает количество копий для печати.

```csharp
public int PrintCopies { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintCopiesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить количество копий печати в 3
            worksheet.PageSetup.PrintCopies = 3;
            
            // Отобразить текущую настройку количества копий печати
            Console.WriteLine("Print Copies: " + worksheet.PageSetup.PrintCopies);
            
            // Сохраните книгу
            workbook.Save("PageSetup_PrintCopies_Output.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


