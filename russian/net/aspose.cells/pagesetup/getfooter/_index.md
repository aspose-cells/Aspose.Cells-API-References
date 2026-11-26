---
title: "PageSetup.GetFooter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Получает скрипт, форматирующий нижний колонтитул файла Excel"
type: docs
url: /ru/net/aspose.cells/pagesetup/getfooter/
---
## PageSetup.GetFooter method

Получает скрипт, форматирующий нижний колонтитул Excel-файла.

```csharp
public string GetFooter(int section)
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
    public class PageSetupMethodGetFooterWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить разные секции нижнего колонтитула
            worksheet.PageSetup.SetFooter(1, "odd");
            worksheet.PageSetup.SetFirstPageFooter(1, "first");
            worksheet.PageSetup.SetEvenFooter(1, "even");

            // Получить и отобразить секции нижнего колонтитула
            Console.WriteLine("First Page Footer: " + worksheet.PageSetup.GetFirstPageFooter(1));
            Console.WriteLine("Even Page Footer: " + worksheet.PageSetup.GetEvenFooter(1));
            Console.WriteLine("Odd Page Footer: " + worksheet.PageSetup.GetFooter(1));
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


