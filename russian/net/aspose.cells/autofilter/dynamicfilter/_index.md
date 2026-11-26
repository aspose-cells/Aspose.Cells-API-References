---
title: "AutoFilter.DynamicFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Добавляет динамический фильтр"
type: docs
url: /ru/net/aspose.cells/autofilter/dynamicfilter/
---
## AutoFilter.DynamicFilter method

Добавляет динамический фильтр.

```csharp
public void DynamicFilter(int fieldIndex, DynamicFilterType dynamicFilterType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | Int32 | Целочисленное смещение поля, на основе которого вы хотите построить фильтр (от левого края списка; самое левое поле имеет индекс 0). |
| dynamicFilterType | DynamicFilterType | Тип динамического фильтра. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodDynamicFilterWithInt32DynamicFilterTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 1));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 5, 1));

            // Примените автофильтр, используя правильную сигнатуру метода
            worksheet.AutoFilter.Range = "A1:A6";

            // Применить динамический фильтр для дат марта
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

            workbook.Save("DynamicFilterDemo.xlsx");
        }
    }
}
```

### См. также

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


