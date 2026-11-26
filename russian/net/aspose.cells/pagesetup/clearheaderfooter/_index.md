---
title: "PageSetup.ClearHeaderFooter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Очищает настройки верхнего и нижнего колонтитулов"
type: docs
url: /ru/net/aspose.cells/pagesetup/clearheaderfooter/
---
## PageSetup.ClearHeaderFooter method

Очищает настройки верхнего и нижнего колонтитулов.

```csharp
public void ClearHeaderFooter()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodClearHeaderFooterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Установить начальные верхние и нижние колонтитулы
            pageSetup.SetHeader(0, "Initial Left Header");
            pageSetup.SetFooter(0, "Initial Left Footer");

            Console.WriteLine("Before ClearHeaderFooter:");
            Console.WriteLine("Header: " + pageSetup.GetHeader(0));
            Console.WriteLine("Footer: " + pageSetup.GetFooter(0));

            // Очистить верхние и нижние колонтитулы
            pageSetup.ClearHeaderFooter();

            Console.WriteLine("\nAfter ClearHeaderFooter:");
            Console.WriteLine("Header: " + (string.IsNullOrEmpty(pageSetup.GetHeader(0)) ? "Cleared" : "Not Cleared"));
            Console.WriteLine("Footer: " + (string.IsNullOrEmpty(pageSetup.GetFooter(0)) ? "Cleared" : "Not Cleared"));

            // Установить новые верхние и нижние колонтитулы после очистки
            pageSetup.SetHeader(0, "New Left Header");
            pageSetup.SetFooter(0, "New Left Footer");

            Console.WriteLine("\nAfter Setting New Values:");
            Console.WriteLine("Header: " + pageSetup.GetHeader(0));
            Console.WriteLine("Footer: " + pageSetup.GetFooter(0));
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


