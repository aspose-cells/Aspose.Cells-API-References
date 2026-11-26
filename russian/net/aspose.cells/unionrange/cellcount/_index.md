---
title: "UnionRange.CellCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство UnionRange. Возвращает общее количество ячеек в диапазоне"
type: docs
url: /ru/net/aspose.cells/unionrange/cellcount/
---
## UnionRange.CellCount property

Получает общее количество ячеек в диапазоне.

```csharp
public int CellCount { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyCellCountDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните данные в листе
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
                }
            }

            // Создайте диапазоны и объедините их в объединённый диапазон
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B3");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("D1:E4");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Отобразите свойство CellCount
            Console.WriteLine("Total cells in union range: " + unionRange.CellCount);

            // Вычислите ожидаемое количество ячеек
            int expectedCount = (range1.RowCount * range1.ColumnCount) + (range2.RowCount * range2.ColumnCount);
            Console.WriteLine("Expected cell count: " + expectedCount);

            // Продемонстрируйте использование, перебирая ячейки
            Console.WriteLine("\nCell values in the union range:");
            int cellCounter = 0;
            foreach (Cell cell in unionRange)
            {
                Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                cellCounter++;
            }

            // Проверьте, что количество ячеек соответствует перебору
            Console.WriteLine($"\nIterated through {cellCounter} cells (should match CellCount)");

            // Создайте ещё один объединённый диапазон с другими размерами
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("A5:E5");
            Aspose.Cells.Range range4 = worksheet.Cells.CreateRange("C1:C5");
            UnionRange unionRange2 = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range3, range4 });

            // Сравните количество ячеек разных объединённых диапазонов
            Console.WriteLine("\nSecond union range cell count: " + unionRange2.CellCount);
            Console.WriteLine("First union range has " + 
                (unionRange.CellCount > unionRange2.CellCount ? "more" : "fewer") + 
                " cells than second union range");

            // Сохраните книгу
            workbook.Save("UnionRangeCellCountDemo.xlsx");
        }
    }
}
```

### См. также

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


