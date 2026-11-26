---
title: "PageSetup.GetHeader"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Получает скрипт, форматирующий заголовок Excel‑файла"
type: docs
url: /ru/net/aspose.cells/pagesetup/getheader/
---
## PageSetup.GetHeader method

Получает скрипт, форматирующий верхний колонтитул Excel-файла.

```csharp
public string GetHeader(int section)
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
    public class PageSetupMethodGetHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите заголовок для секции 2
            worksheet.PageSetup.SetHeader(2, "&8Report ID: TEST01\n你好Public");
            
            // Получите и выведите заголовок для секции 2
            string header = worksheet.PageSetup.GetHeader(2);
            Console.WriteLine("Header for section 2: " + header);
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


