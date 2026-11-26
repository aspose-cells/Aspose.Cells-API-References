---
title: "PivotTableFormatCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "PivotTableFormatCollection свойство. Получает формат по индексу"
type: docs
url: /ru/net/aspose.cells.pivot/pivottableformatcollection/item/
---
## PivotTableFormatCollection indexer

Получает формат по индексу.

```csharp
public PivotTableFormat this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("example.xlsx");

            // Обновить все сводные таблицы
            workbook.Worksheets.RefreshAll();
            Cells cells = workbook.Worksheets[0].Cells;

            // Получить доступ к первой сводной таблице.
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];

            // Продемонстрировать свойство Item, получив первый PivotFormat
            pt.PivotFormats[0].PivotArea.OnlyData = false;
            workbook.Worksheets.RefreshAll();

            // Изменить параметры формата, используя свойство Item
            pt.PivotFormats[0].PivotArea.OnlyLabel = true;
            workbook.Worksheets.RefreshAll();

            // Сохранить изменённую книгу
            workbook.Save("modified_example.xlsx");
        }
    }
}
```

### См. также

* class [PivotTableFormat](../../pivottableformat/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


