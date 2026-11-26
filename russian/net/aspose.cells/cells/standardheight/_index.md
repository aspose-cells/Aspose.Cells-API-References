---
title: "Cells.StandardHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Получает или задаёт высоту строки по умолчанию в этом листе в единицах точек"
type: docs
url: /ru/net/aspose.cells/cells/standardheight/
---
## Cells.StandardHeight property

Получает или задает высоту строки по умолчанию в этом листе, в единицах пунктов.

```csharp
public double StandardHeight { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить и отобразить стандартную высоту
            double standardHeight = worksheet.Cells.StandardHeight;
            Console.WriteLine("Standard Height: " + standardHeight);
            
            // Установить новую стандартную высоту
            worksheet.Cells.StandardHeight = 20;
            Console.WriteLine("New Standard Height: " + worksheet.Cells.StandardHeight);
            
            // Сохраните книгу
            workbook.Save("StandardHeightDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


