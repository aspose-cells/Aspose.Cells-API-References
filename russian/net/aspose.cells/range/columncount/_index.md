---
title: "Range.ColumnCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Возвращает количество столбцов в диапазоне"
type: docs
url: /ru/net/aspose.cells/range/columncount/
---
## Range.ColumnCount property

Получает количество столбцов в диапазоне.

```csharp
public int ColumnCount { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyColumnCountDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Создайте примерные данные (5 столбцов × 3 строки)
            for (int col = 0; col < 5; col++)
            {
                for (int row = 0; row < 3; row++)
                {
                    sheet.Cells[row, col].PutValue($"Data {row},{col}");
                }
            }
            
            // Создайте диапазон, охватывающий все столбцы данных
            Aspose.Cells.Range dataRange = sheet.Cells.CreateRange(0, 0, 3, 5);
            
            // Продемонстрируйте использование ColumnCount
            Console.WriteLine($"Range has {dataRange.ColumnCount} columns");
            
            // Автоматически подгоните каждый столбец в диапазоне
            for (int i = 0; i < dataRange.ColumnCount; i++)
            {
                sheet.AutoFitColumn(dataRange.FirstColumn + i);
            }
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


