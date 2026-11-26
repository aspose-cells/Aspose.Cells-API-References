---
title: "Range.IsIntersect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Указывает, пересекается ли диапазон"
type: docs
url: /ru/net/aspose.cells/range/isintersect/
---
## Range.IsIntersect method

Указывает, пересекается ли диапазон.

```csharp
public bool IsIntersect(Range range)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазон | Диапазон | Диапазон. |

### Возвращаемое значение

Пересекается ли диапазон.

### Примечания

Если два диапазона находятся не в одном листе, вернуть false.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodIsIntersectWithRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте два диапазона для тестирования пересечения
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B3:D8");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("C10:D15");

            try
            {
                // Проверьте, пересекается ли range1 с range2 (должно пересекаться)
                bool result1 = range1.IsIntersect(range2);
                Console.WriteLine($"Range A1:B5 intersects with B3:D8: {result1}");

                // Проверьте, пересекается ли range1 с range3 (не должно пересекаться)
                bool result2 = range1.IsIntersect(range3);
                Console.WriteLine($"Range A1:B5 intersects with C10:D15: {result2}");

                // Заполните диапазоны разными цветами для их визуализации
                Style style1 = workbook.CreateStyle();
                style1.ForegroundColor = System.Drawing.Color.LightBlue;
                style1.Pattern = BackgroundType.Solid;
                range1.SetStyle(style1);

                Style style2 = workbook.CreateStyle();
                style2.ForegroundColor = System.Drawing.Color.LightGreen;
                style2.Pattern = BackgroundType.Solid;
                range2.SetStyle(style2);

                Style style3 = workbook.CreateStyle();
                style3.ForegroundColor = System.Drawing.Color.LightPink;
                style3.Pattern = BackgroundType.Solid;
                range3.SetStyle(style3);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsIntersect method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("RangeMethodIsIntersectWithRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


