---
title: "Range.CopyValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Копирует значение ячейки из исходного диапазона"
type: docs
url: /ru/net/aspose.cells/range/copyvalue/
---
## Range.CopyValue method

Копирует значение ячейки из исходного диапазона.

```csharp
public void CopyValue(Range range)
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
    public class RangeMethodCopyValueWithRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте лист и получите первый лист
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "SourceSheet";
            
            // Добавить еще один лист для назначения
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "DestinationSheet";
            
            // Создать примерные данные в исходном диапазоне
            Cells cellsSrc = sheetSrc.Cells;
            cellsSrc["A1"].PutValue("Source Data");
            cellsSrc["A2"].PutValue(10);
            cellsSrc["B2"].PutValue(20);
            cellsSrc["A3"].PutValue(30);
            cellsSrc["B3"].PutValue(40);
            
            // Создать диапазоны для исходного и целевого
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A2:B3");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("D2:E3");
            
            // Копировать значения из исходного диапазона в целевой диапазон
            rangeDest.CopyValue(rangeSrc);
            
            // Сохраните книгу
            workbook.Save("RangeCopyValueDemo.xlsx");
            
            Console.WriteLine("Values copied successfully from source range to destination range.");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


