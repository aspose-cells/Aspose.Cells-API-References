---
title: "PageSetup.GetEvenHeader"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Получает скрипт, форматирующий чётный заголовок Excel‑файла"
type: docs
url: /ru/net/aspose.cells/pagesetup/getevenheader/
---
## PageSetup.GetEvenHeader method

Получает скрипт, форматирующий четный верхний колонтитул Excel-файла.

```csharp
public string GetEvenHeader(int section)
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
    public class PageSetupMethodGetEvenHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Включить разные нечётные и чётные колонтитулы страниц
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.IsHFDiffOddEven = true;
            
            // Установить чётный заголовок страницы
            pageSetup.SetEvenHeader(0, "&CEven Page Header Center");
            pageSetup.SetEvenHeader(1, "&LEven Page Header Left");
            pageSetup.SetEvenHeader(2, "&REven Page Header Right");
            
            // Получить и вывести чётные заголовки страниц
            Console.WriteLine("Even Header Center: " + pageSetup.GetEvenHeader(0));
            Console.WriteLine("Even Header Left: " + pageSetup.GetEvenHeader(1));
            Console.WriteLine("Even Header Right: " + pageSetup.GetEvenHeader(2));
            
            // Сохраните книгу
            workbook.Save("PageSetup_GetEvenHeaderDemo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


