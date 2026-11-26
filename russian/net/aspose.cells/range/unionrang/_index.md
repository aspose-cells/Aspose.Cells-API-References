---
title: "Range.UnionRang"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Возвращает результат объединения двух диапазонов"
type: docs
url: /ru/net/aspose.cells/range/unionrang/
---
## Range.UnionRang method

Возвращает результат объединения двух диапазонов.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Range[] UnionRang(Range range)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазон | Диапазон | Диапазон |

### Возвращаемое значение

Объединение двух диапазонов.

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Range.UnionRanges(). Этот метод будет удалён через 12 месяцев, начиная с мая 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using Range = Aspose.Cells.Range; // Add this alias to resolve ambiguity

    public class RangeMethodUnionRangWithRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте два диапазона для демонстрации UnionRang
            Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Range range2 = worksheet.Cells.CreateRange("C3:D4");

            // Установите некоторые значения в диапазонах для визуализации
            range1[0, 0].PutValue("Range1");
            range1[1, 1].PutValue("Data");
            range2[0, 0].PutValue("Range2");
            range2[1, 1].PutValue("Data");

            try
            {
                // Вызовите метод UnionRang, чтобы объединить два диапазона
                Range[] unionResult = range1.UnionRang(range2);

                // Отобразите информацию о результате объединения
                Console.WriteLine("UnionRang method executed successfully.");
                Console.WriteLine($"Number of ranges in union: {unionResult.Length}");
                Console.WriteLine($"First union range address: {unionResult[0].Address}");
                Console.WriteLine($"Second union range address: {unionResult[1].Address}");

                // Отметьте объединённые диапазоны границей для визуализации
                foreach (Range r in unionResult)
                {
                    r.SetOutlineBorders(CellBorderType.Thin, System.Drawing.Color.Black);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRang method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("RangeMethodUnionRangWithRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


