---
title: "PageSetup.Order"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет порядок, который Microsoft Excel использует для нумерации страниц при печати большого листа."
type: docs
url: /ru/net/aspose.cells/pagesetup/order/
---
## PageSetup.Order property

Представляет порядок, который Microsoft Excel использует для нумерации страниц при печати большого листа.

```csharp
public PrintOrderType Order { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrderDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Установить порядок печати в DownThenOver
            sheet.PageSetup.Order = PrintOrderType.DownThenOver;
            Console.WriteLine("Print order set to: " + sheet.PageSetup.Order);

            // Сохранить книгу в разных форматах
            workbook.Save("output_DownThenOver.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_DownThenOver.xls", SaveFormat.Excel97To2003);

            // Измените порядок печати на OverThenDown
            sheet.PageSetup.Order = PrintOrderType.OverThenDown;
            Console.WriteLine("Print order changed to: " + sheet.PageSetup.Order);

            // Сохраните снова в разных форматах
            workbook.Save("output_OverThenDown.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_OverThenDown.xls", SaveFormat.Excel97To2003);
        }
    }
}
```

### См. также

* enum [PrintOrderType](../../printordertype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


