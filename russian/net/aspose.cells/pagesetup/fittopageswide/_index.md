---
title: "PageSetup.FitToPagesWide"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет количество страниц по ширине, до которого будет масштабироваться лист при печати. Значение по умолчанию — 1"
type: docs
url: /ru/net/aspose.cells/pagesetup/fittopageswide/
---
## PageSetup.FitToPagesWide property

Представляет количество страниц по ширине, до которого будет масштабироваться лист при печати. Значение по умолчанию — 1.

```csharp
public int FitToPagesWide { get; set; }
```

### Примечания

Необходимо установить FitToPagesTall в ноль, если вы хотите разместить все столбцы на одной странице.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesWideDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Sample Data 1");
            worksheet.Cells["A2"].PutValue("Sample Data 2");
            worksheet.Cells["B1"].PutValue("Sample Data 3");
            worksheet.Cells["B2"].PutValue("Sample Data 4");

            // Установить свойства настройки страницы
            worksheet.PageSetup.FitToPagesWide = 1;  // Fit to 1 page wide
            worksheet.PageSetup.FitToPagesTall = 0; // Let height adjust automatically

            // Сохраните книгу
            workbook.Save("FitToPagesWideDemo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


