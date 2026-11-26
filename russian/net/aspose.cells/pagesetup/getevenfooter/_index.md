---
title: "PageSetup.GetEvenFooter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Получает скрипт, форматирующий нижний колонтитул чётных страниц Excel‑файла"
type: docs
url: /ru/net/aspose.cells/pagesetup/getevenfooter/
---
## PageSetup.GetEvenFooter method

Получает скрипт, форматирующий четный нижний колонтитул Excel-файла.

```csharp
public string GetEvenFooter(int section)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| секция | Int32 | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetEvenFooterWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Включить разные верхние и нижние колонтитулы для нечётных и чётных страниц
            pageSetup.IsHFDiffOddEven = true;
            
            // Установить нижний колонтитул чётных страниц
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // Получить и отобразить нижний колонтитул чётных страниц
            string evenFooter = pageSetup.GetEvenFooter(0);
            Console.WriteLine("Even Footer: " + evenFooter);
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


