---
title: "Cells.StandardWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Получает или задает ширину столбца по умолчанию в листе в единицах символов"
type: docs
url: /ru/net/aspose.cells/cells/standardwidth/
---
## Cells.StandardWidth property

Получает или задает ширину столбца по умолчанию в листе, в единицах символов.

```csharp
public double StandardWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить стандартную ширину для столбцов
            cells.StandardWidth = 18.25;

            // Отобразить стандартную ширину и фактическую ширину первого столбца
            Console.WriteLine("Standard Width: " + cells.StandardWidth);
            Console.WriteLine("Column 0 Width: " + cells.GetColumnWidth(0));

            // Проверить, что стандартная ширина применена (примерно)
            if (Math.Abs(cells.GetColumnWidth(0) - cells.StandardWidth) > 1.0)
            {
                Console.WriteLine("Warning: Column width differs significantly from standard width");
            }
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


