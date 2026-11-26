---
title: "PageSetup.IsHFDiffFirst"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. True означает, что верхний/нижний колонтитул первой страницы отличается от остальных страниц"
type: docs
url: /ru/net/aspose.cells/pagesetup/ishfdifffirst/
---
## PageSetup.IsHFDiffFirst property

True означает, что верхний/нижний колонтитул первой страницы отличается от остальных страниц.

```csharp
public bool IsHFDiffFirst { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffFirstDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Доступ к PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Установить разные верхние/нижние колонтитулы для первой страницы
            pageSetup.IsHFDiffFirst = true;
            
            // Установить колонтитулы
            pageSetup.SetFirstPageHeader(0, "First Page Header");
            pageSetup.SetHeader(0, "Standard Header");
            
            // Сохраните книгу
            workbook.Save("PageSetup_IsHFDiffFirst_Example.xlsx");
            
            // Перезагрузите книгу, чтобы проверить настройки
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffFirst_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            // Вывести проверку
            Console.WriteLine("IsHFDiffFirst: " + loadedPageSetup.IsHFDiffFirst);
            Console.WriteLine("First Page Header: " + loadedPageSetup.GetFirstPageHeader(0));
            Console.WriteLine("Standard Header: " + loadedPageSetup.GetHeader(0));
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


