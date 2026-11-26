---
title: "Range.UnionRanges"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Возвращает результат объединения двух диапазонов"
type: docs
url: /ru/net/aspose.cells/range/unionranges/
---
## Range.UnionRanges method

Возвращает результат объединения двух диапазонов.

```csharp
public UnionRange UnionRanges(Range[] ranges)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазоны | Range[] | Диапазон |

### Возвращаемое значение

Объединение двух диапазонов.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodUnionRangesWithRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте пример данных в ячейках
            worksheet.Cells["A1"].PutValue("Range 1");
            worksheet.Cells["B1"].PutValue("Data 1");
            worksheet.Cells["C1"].PutValue("Data 2");
            worksheet.Cells["A5"].PutValue("Range 2");
            worksheet.Cells["B5"].PutValue("Data 3");
            worksheet.Cells["C5"].PutValue("Data 4");

            // Создайте диапазоны для объединения
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C3");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A5:C7");

            try
            {
                // Вызовите UnionRanges с параметром Range[]
                Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range1, range2 };
                UnionRange unionRange = range1.UnionRanges(rangesToUnion);

                // Примените стиль, чтобы показать объединённый диапазон
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });

                Console.WriteLine($"Union range created successfully. Address: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRanges method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("UnionRangesDemo.xlsx");
        }
    }
}
```

### См. также

* class [UnionRange](../../unionrange/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


