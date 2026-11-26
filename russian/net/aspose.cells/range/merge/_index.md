---
title: "Range.Merge"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Объединяет диапазон ячеек в одну ячейку"
type: docs
url: /ru/net/aspose.cells/range/merge/
---
## Range.Merge method

Объединяет диапазон ячеек в одну ячейку.

```csharp
public void Merge()
```

### Примечания

Ссылайтесь на объединённую ячейку через адрес верхней‑левой ячейки в диапазоне.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMergeDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте диапазон и объедините ячейки (3 строки × 2 столбца)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            range.Merge();

            // Установите значение в объединённой ячейке
            worksheet.Cells[0, 0].Value = "Merged Cells Demo";

            // Примените стиль к объединённым ячейкам
            Style style = worksheet.Cells[0, 0].GetStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.IsBold = true;
            worksheet.Cells[0, 0].SetStyle(style);

            // Сохраните книгу
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


