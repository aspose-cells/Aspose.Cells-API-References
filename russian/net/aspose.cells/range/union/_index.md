---
title: "Range.Union"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Возвращает объединение двух диапазонов"
type: docs
url: /ru/net/aspose.cells/range/union/
---
## Range.Union method

Возвращает объединение двух диапазонов.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList Union(Range range)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазон | Диапазон | Диапазон |

### Возвращаемое значение

Объединение двух диапазонов.

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Range.UnionRanges(). Этот метод будет удалён через 12 месяцев, начиная с ноября 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RangeMethodUnionWithRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте два диапазона, чтобы продемонстрировать Union
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:C3");

            // Заполните некоторые данные в диапазонах
            range1[0, 0].PutValue("Range1");
            range2[0, 0].PutValue("Range2");

            try
            {
                // Вызовите метод Union (примечание: это устаревшая версия)
                ArrayList unionResult = range1.Union(range2);

                Console.WriteLine("Union method executed successfully");
                Console.WriteLine($"Number of ranges in union: {unionResult.Count}");

                // Отобразите адреса всех диапазонов в объединении
                foreach (Aspose.Cells.Range r in unionResult)
                {
                    Console.WriteLine($"Union range address: {r.Address}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("RangeMethodUnionWithRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


