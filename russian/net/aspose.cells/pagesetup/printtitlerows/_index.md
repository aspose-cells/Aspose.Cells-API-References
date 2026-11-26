---
title: "PageSetup.PrintTitleRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет строки, содержащие ячейки, которые повторяются в верхней части каждой страницы"
type: docs
url: /ru/net/aspose.cells/pagesetup/printtitlerows/
---
## PageSetup.PrintTitleRows property

Отображает строки, содержащие ячейки, которые повторяются в верхней части каждой страницы.

```csharp
public string PrintTitleRows { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleRowsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите некоторые примерные данные
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Data " + (i-1));
            }
            
            // Доступ к настройкам страницы
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Установить строки заголовков для печати (первая строка будет повторяться на каждой печатной странице)
            pageSetup.PrintTitleRows = "$1:$1";
            
            // Сохраните книгу
            workbook.Save("PrintTitleRowsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


