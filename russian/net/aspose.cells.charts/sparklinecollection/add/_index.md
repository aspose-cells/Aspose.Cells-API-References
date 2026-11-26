---
title: "SparklineCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SparklineCollection. Добавить спарклайн"
type: docs
url: /ru/net/aspose.cells.charts/sparklinecollection/add/
---
## SparklineCollection.Add method

Добавить спарклайн.

```csharp
public int Add(string dataRange, int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dataRange | String | Указывает новый диапазон данных спарклайна. |
| строка | Int32 | Индекс строки расположения. |
| column | Int32 | Индекс столбца расположения. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            for (int i = 0; i < 12; i++)
            {
                worksheet.Cells[4, 3 + i].PutValue(i + 1);
            }

            // Создать группу спарклайнов
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Добавить спарклайн с диапазоном данных и расположением
            int sparklineIndex = group.Sparklines.Add("D5:O5", 4, 15);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


