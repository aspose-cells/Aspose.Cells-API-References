---
title: "PageSetup.SetEvenFooter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Устанавливает скрипт форматирования нижнего колонтитула четных страниц Excel‑файла. Действует только в Excel 2007, когда IsHFDiffOddEven равно true"
type: docs
url: /ru/net/aspose.cells/pagesetup/setevenfooter/
---
## PageSetup.SetEvenFooter method

Устанавливает скрипт, форматирующий четный нижний колонтитул страницы Excel-файла. Действует только в Excel 2007, когда IsHFDiffOddEven равно true.

```csharp
public void SetEvenFooter(int section, string footerScript)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| секция | Int32 | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| footerScript | String | Скрипт формата нижнего колонтитула. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetEvenFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Включить разные колонтитулы для первой и четных страниц
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;

            // Установить разные типы нижних колонтитулов
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetFirstPageFooter(0, "First Page Footer");

            // Сохраните книгу
            workbook.Save("PageSetup_SetEvenFooter_Example.xlsx");

            Console.WriteLine("Workbook saved with even page footer set successfully.");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


