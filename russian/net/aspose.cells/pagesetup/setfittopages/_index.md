---
title: "PageSetup.SetFitToPages"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Устанавливает количество страниц, до которых будет масштабирован лист при печати."
type: docs
url: /ru/net/aspose.cells/pagesetup/setfittopages/
---
## PageSetup.SetFitToPages method

Устанавливает количество страниц, до которых будет масштабироваться лист при печати.

```csharp
public void SetFitToPages(int wide, int tall)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| широкий | Int32 | Страниц в ширину. |
| высокий | Int32 | Страниц в высоту. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFitToPagesWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Обратиться к PageSetup первого листа
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // Установите настройки подгонки к страницам
            setup.SetFitToPages(2, 3);
            
            // Проверьте и выведите настройки
            Console.WriteLine("IsPercentScale: " + setup.IsPercentScale);
            Console.WriteLine("FitToPagesWide: " + setup.FitToPagesWide);
            Console.WriteLine("FitToPagesTall: " + setup.FitToPagesTall);
            
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


