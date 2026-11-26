---
title: "PageSetup.Zoom"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет коэффициент масштабирования в процентах. Должно быть от 10 до 400"
type: docs
url: /ru/net/aspose.cells/pagesetup/zoom/
---
## PageSetup.Zoom property

Отображает коэффициент масштабирования в процентах. Он должен быть от 10 до 400.

```csharp
public int Zoom { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyZoomDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите уровень масштабирования на 150%
            worksheet.PageSetup.Zoom = 150;
            
            // Выведите текущий уровень масштабирования
            Console.WriteLine("Current Zoom Level: " + worksheet.PageSetup.Zoom);
            
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


