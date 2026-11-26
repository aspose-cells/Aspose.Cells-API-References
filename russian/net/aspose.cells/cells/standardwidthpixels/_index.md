---
title: "Cells.StandardWidthPixels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Получает или задаёт ширину столбца по умолчанию в листе в единицах пикселей"
type: docs
url: /ru/net/aspose.cells/cells/standardwidthpixels/
---
## Cells.StandardWidthPixels property

Получает или задает ширину столбца по умолчанию в листе, в единицах пикселей.

```csharp
public int StandardWidthPixels { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthPixelsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить и получить стандартную ширину в пикселях
            cells.StandardWidthPixels = 104;
            Console.WriteLine("Standard Width in Pixels: " + cells.StandardWidthPixels);

            // Установить и получить стандартную ширину в символах
            cells.StandardWidth = 12.375;
            Console.WriteLine("Standard Width in Characters: " + cells.StandardWidth);

            // Установить и получить стандартную высоту в пунктах
            cells.StandardHeight = 14.25;
            Console.WriteLine("Standard Height in Points: " + cells.StandardHeight);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


