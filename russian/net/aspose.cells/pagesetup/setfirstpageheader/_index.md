---
title: "PageSetup.SetFirstPageHeader"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Устанавливает скрипт, форматирующий верхний колонтитул первой страницы Excel‑файла. Действует только в Excel 2007, когда IsHFDiffFirst равно true"
type: docs
url: /ru/net/aspose.cells/pagesetup/setfirstpageheader/
---
## PageSetup.SetFirstPageHeader method

Устанавливает скриптовое форматирование верхнего колонтитула первой страницы Excel‑файла. Действует только в Excel 2007, когда IsHFDiffFirst равно true.

```csharp
public void SetFirstPageHeader(int section, string headerScript)
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
    public class PageSetupMethodSetFirstPageHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Установить верхний колонтитул первой страницы с номером раздела и текстом заголовка
            pageSetup.SetFirstPageHeader(2, "&CHeader Text");

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


