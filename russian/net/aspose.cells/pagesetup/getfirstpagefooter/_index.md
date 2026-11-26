---
title: "PageSetup.GetFirstPageFooter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Получает скрипт, форматирующий нижний колонтитул первой страницы Excel‑файла"
type: docs
url: /ru/net/aspose.cells/pagesetup/getfirstpagefooter/
---
## PageSetup.GetFirstPageFooter method

Получает скрипт, форматирующий нижний колонтитул первой страницы Excel-файла.

```csharp
public string GetFirstPageFooter(int section)
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
    public class PageSetupMethodGetFirstPageFooterWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить нижний колонтитул первой страницы
            worksheet.PageSetup.SetFirstPageFooter(1, "First Page Footer");

            // Получить и вывести нижний колонтитул первой страницы
            string footer = worksheet.PageSetup.GetFirstPageFooter(1);
            Console.WriteLine("First Page Footer: " + footer);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


