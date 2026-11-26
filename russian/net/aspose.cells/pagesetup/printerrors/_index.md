---
title: "PageSetup.PrintErrors"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Указывает тип отображаемой ошибки печати"
type: docs
url: /ru/net/aspose.cells/pagesetup/printerrors/
---
## PageSetup.PrintErrors property

Указывает тип отображаемой ошибки печати.

```csharp
public PrintErrorsType PrintErrors { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintErrorsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Установить отображение ошибок печати как пустое
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            Console.WriteLine("PrintErrors set to: " + sheet.PageSetup.PrintErrors);
            
            // Изменить отображение ошибок печати на тире
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            Console.WriteLine("PrintErrors changed to: " + sheet.PageSetup.PrintErrors);
            
            // Сохраните книгу
            workbook.Save("PrintErrorsDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PrintErrorsType](../../printerrorstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


