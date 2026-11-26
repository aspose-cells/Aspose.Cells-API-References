---
title: "PageSetup.PrintGridlines"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Указывает, печатаются ли линии сетки ячеек на странице"
type: docs
url: /ru/net/aspose.cells/pagesetup/printgridlines/
---
## PageSetup.PrintGridlines property

Отображает, печатаются ли линии сетки ячеек на странице.

```csharp
public bool PrintGridlines { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintGridlinesDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Поместить примерные данные в ячейку
            worksheet.Cells["A1"].PutValue("PrintGridlines Property Demo");
            worksheet.Cells["A3"].PutValue("Gridlines will ");
            worksheet.Cells["B3"].PutValue(worksheet.PageSetup.PrintGridlines ? "appear" : "not appear");
            worksheet.Cells["A4"].PutValue("when printing this sheet.");

            // Переключить свойство PrintGridlines
            worksheet.PageSetup.PrintGridlines = true;
            
            // Сохраните книгу
            workbook.Save("PrintGridlinesDemo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


