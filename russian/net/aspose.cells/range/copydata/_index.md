---
title: "Range.CopyData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Копирует данные ячеек, включая формулы, из исходного диапазона"
type: docs
url: /ru/net/aspose.cells/range/copydata/
---
## Range.CopyData method

Копирует данные ячейки (включая формулы) из исходного диапазона.

```csharp
public void CopyData(Range range)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| range | Range | Исходный объект [`Range`](../). |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyDataWithRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите первый лист и добавьте некоторые данные
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            sheetSrc.Cells["A1"].PutValue("Source Data");
            sheetSrc.Cells["B1"].PutValue(100);
            sheetSrc.Cells["A2"].PutValue("More Data");
            sheetSrc.Cells["B2"].PutValue(200);

            // Добавьте лист назначения
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";

            // Создайте исходные и целевые диапазоны
            Aspose.Cells.Range rangeSrc = sheetSrc.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("C3:D4");

            // Скопируйте данные из исходного диапазона в целевой диапазон
            rangeDest.CopyData(rangeSrc);

            // Сохраните книгу
            workbook.Save("RangeCopyDataDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


