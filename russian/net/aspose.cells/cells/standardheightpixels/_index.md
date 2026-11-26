---
title: "Cells.StandardHeightPixels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Получает или задает высоту строки по умолчанию в этом листе в единицах пикселей"
type: docs
url: /ru/net/aspose.cells/cells/standardheightpixels/
---
## Cells.StandardHeightPixels property

Получает или задает высоту строки по умолчанию в этом листе, в единицах пикселей.

```csharp
public int StandardHeightPixels { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightPixelsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить некоторые данные в ячейки
            cells["A1"].PutValue("Sample Data");
            cells["B2"].PutValue(123);
            cells["C3"].PutValue(DateTime.Now);

            // Получить стандартную высоту в пикселях
            int standardHeight = cells.StandardHeightPixels;
            Console.WriteLine("Standard row height in pixels: " + standardHeight);

            // Отобразить высоты строк (должны соответствовать стандартной высоте)
            for (int i = 0; i < 5; i++)
            {
                int rowHeight = cells.GetRowHeightPixel(i);
                Console.WriteLine($"Row {i} height: {rowHeight}px");
                Console.WriteLine($"Matches standard: {rowHeight == standardHeight}");
            }

            // Изменить стандартную высоту и проверить
            cells.StandardHeight = 20; // Set in points
            int newStandardHeight = cells.StandardHeightPixels;
            Console.WriteLine("\nNew standard height in pixels: " + newStandardHeight);

            // Проверить, что все строки теперь имеют новую высоту
            for (int i = 0; i < 5; i++)
            {
                int rowHeight = cells.GetRowHeightPixel(i);
                Console.WriteLine($"Row {i} height: {rowHeight}px");
                Console.WriteLine($"Matches new standard: {rowHeight == newStandardHeight}");
            }
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


