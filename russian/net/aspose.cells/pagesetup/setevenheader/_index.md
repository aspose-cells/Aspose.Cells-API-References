---
title: "PageSetup.SetEvenHeader"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Устанавливает скрипт, форматирующий верхний колонтитул чётных страниц Excel‑файла. Действует только в Excel 2007, когда IsHFDiffOddEven равно true"
type: docs
url: /ru/net/aspose.cells/pagesetup/setevenheader/
---
## PageSetup.SetEvenHeader method

Устанавливает скрипт, форматирующий четный верхний колонтитул страницы Excel-файла. Действует только в Excel 2007, когда IsHFDiffOddEven равно true.

```csharp
public void SetEvenHeader(int section, string headerScript)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| секция | Int32 | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| headerScript | String | Скрипт формата заголовка. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetEvenHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Включить разные верхние и нижние колонтитулы для нечётных и чётных страниц
            pageSetup.IsHFDiffOddEven = true;

            // Установить верхний колонтитул чётных страниц с индексом раздела и текстом
            pageSetup.SetEvenHeader(1, "Even Page Header - Center Section");
            pageSetup.SetEvenHeader(0, "Even Page Header - Left Section");
            pageSetup.SetEvenHeader(2, "Even Page Header - Right Section");

            // Сохраните книгу
            workbook.Save("PageSetup_SetEvenHeaderExample.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


