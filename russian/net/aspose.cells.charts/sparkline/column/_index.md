---
title: "Sparkline.Column"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Sparkline. Возвращает индекс столбца спарклайна"
type: docs
url: /ru/net/aspose.cells.charts/sparkline/column/
---
## Sparkline.Column property

Получает индекс столбца спарклайна.

```csharp
public int Column { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Создать группу спарклайнов
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            
            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];

            // Добавьте спарклайн в столбец 4 и продемонстрируйте свойство Column
            int sparklineIndex = group.Sparklines.Add("A1:D1", 0, 4);
            Sparkline sparkline = group.Sparklines[sparklineIndex];

            // Отобразите свойство столбца (только для чтения)
            Console.WriteLine("Sparkline Column: " + sparkline.Column);

            // Чтобы изменить позицию столбца, необходимо удалить и заново добавить спарклайн
            group.Sparklines.RemoveAt(sparklineIndex);
            sparklineIndex = group.Sparklines.Add("A1:D1", 0, 5); // New column position
            sparkline = group.Sparklines[sparklineIndex];
            Console.WriteLine("New Sparkline Column: " + sparkline.Column);

            // Сохранить книгу
            workbook.Save("SparklineColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


