---
title: "PageSetup.IsHFDiffOddEven"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. True означает, что верхний/нижний колонтитул нечётных страниц отличается от колонтитулов чётных страниц"
type: docs
url: /ru/net/aspose.cells/pagesetup/ishfdiffoddeven/
---
## PageSetup.IsHFDiffOddEven property

True означает, что верхний/нижний колонтитул нечётных страниц отличается от нечётных страниц.

```csharp
public bool IsHFDiffOddEven { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffOddEvenDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Доступ к PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Включить разные верхние и нижние колонтитулы для нечётных и чётных страниц
            pageSetup.IsHFDiffOddEven = true;
            
            // Установить разные нижние колонтитулы для нечётных и чётных страниц
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // Сохраните книгу
            workbook.Save("PageSetup_IsHFDiffOddEven_Example.xlsx");
            
            // Проверьте настройки, загрузив сохранённый файл
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffOddEven_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            Console.WriteLine("IsHFDiffOddEven: " + loadedPageSetup.IsHFDiffOddEven);
            Console.WriteLine("Odd Page Footer: " + loadedPageSetup.GetFooter(0));
            Console.WriteLine("Even Page Footer: " + loadedPageSetup.GetEvenFooter(0));
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


