---
title: "PageSetup.GetFirstPageHeader"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Получает скрипт, форматирующий заголовок первой страницы Excel‑файла"
type: docs
url: /ru/net/aspose.cells/pagesetup/getfirstpageheader/
---
## PageSetup.GetFirstPageHeader method

Получает скрипт, форматирующий верхний колонтитул первой страницы Excel-файла.

```csharp
public string GetFirstPageHeader(int section)
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
    public class PageSetupMethodGetFirstPageHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Доступ к PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Включить отдельный заголовок/нижний колонтитул первой страницы
            pageSetup.IsHFDiffFirst = true;
            
            // Установить секции заголовка первой страницы
            pageSetup.SetFirstPageHeader(0, "&LFirst Page Left Header");
            pageSetup.SetFirstPageHeader(1, "&CFirst Page Center Header");
            pageSetup.SetFirstPageHeader(2, "&RFirst Page Right Header");
            
            // Получить и отобразить секции заголовка первой страницы
            Console.WriteLine("First Page Header Sections:");
            Console.WriteLine("Left: " + pageSetup.GetFirstPageHeader(0));
            Console.WriteLine("Center: " + pageSetup.GetFirstPageHeader(1));
            Console.WriteLine("Right: " + pageSetup.GetFirstPageHeader(2));
            
            // Сохраните книгу
            workbook.Save("PageSetupFirstPageHeaderDemo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


