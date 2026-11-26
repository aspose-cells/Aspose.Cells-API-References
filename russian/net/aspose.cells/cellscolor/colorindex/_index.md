---
title: "CellsColor.ColorIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellsColor. Получает и задает индекс цвета в палитре. Применяется только к индексированным цветам"
type: docs
url: /ru/net/aspose.cells/cellscolor/colorindex/
---
## CellsColor.ColorIndex property

Получает и задает индекс цвета в палитре. Применяется только для индексированных цветов.

```csharp
public int ColorIndex { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class CellsColorPropertyColorIndexDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Определите диапазон, к которому будет применена цветная граница
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // Создать экземпляр CellsColor
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Установите ColorIndex (индекс палитры) — например, 5
            cellsColor.ColorIndex = 5;

            // Примените CellsColor в качестве цвета внутренней границы диапазона
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical,
                                   CellBorderType.Thin,
                                   cellsColor);

            // Прочитать и отобразить текущее значение ColorIndex
            Console.WriteLine("Current ColorIndex value: " + cellsColor.ColorIndex);

            // Сохраните книгу, чтобы визуализировать результат
            try
            {
                workbook.Save("ColorIndexDemo.xlsx");
                Console.WriteLine("Workbook saved as ColorIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


