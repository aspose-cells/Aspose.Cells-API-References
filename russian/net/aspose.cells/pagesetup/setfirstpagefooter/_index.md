---
title: "PageSetup.SetFirstPageFooter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Устанавливает скрипт, форматирующий нижний колонтитул первой страницы Excel‑файла"
type: docs
url: /ru/net/aspose.cells/pagesetup/setfirstpagefooter/
---
## PageSetup.SetFirstPageFooter method

Устанавливает скрипт, форматирующий нижний колонтитул первой страницы Excel-файла.

```csharp
public void SetFirstPageFooter(int section, string footerScript)
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
    public class PageSetupMethodSetFirstPageFooterWithInt32StringDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить объект PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Установить разные верхние/нижние колонтитулы для первой страницы
            pageSetup.IsHFDiffFirst = true;
            
            // Установить нижний колонтитул первой страницы с индексом раздела и текстом
            pageSetup.SetFirstPageFooter(0, "First Page Footer Text");
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            Console.WriteLine("First page footer set successfully.");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


