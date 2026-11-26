---
title: "Worksheet.Zoom"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Представляет коэффициент масштабирования в процентах. Должно быть от 10 до 400"
type: docs
url: /ru/net/aspose.cells/worksheet/zoom/
---
## Worksheet.Zoom property

Представляет коэффициент масштабирования в процентах. Должен быть в диапазоне от 10 до 400.

```csharp
public int Zoom { get; set; }
```

### Примечания

Пожалуйста, сначала установите тип представления.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyZoomDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите коэффициент масштабирования на 120%
            worksheet.Zoom = 120;
            
            // Отобразить текущий коэффициент масштабирования
            Console.WriteLine("Current worksheet zoom: " + worksheet.Zoom + "%");
            
            // Сохраните книгу
            workbook.Save("WorksheetZoomDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


