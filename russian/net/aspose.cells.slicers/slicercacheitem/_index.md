---
title: "Класс SlicerCacheItem"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Slicers.SlicerCacheItem. Представляет элемент источника данных slicer"
type: docs
url: /ru/net/aspose.cells.slicers/slicercacheitem/
---
## SlicerCacheItem class

Представляет элемент источника данных среза

```csharp
public class SlicerCacheItem
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Selected](../../aspose.cells.slicers/slicercacheitem/selected/) { get; set; } | Указывает, выбран ли `SlicerCacheItem` или нет. |
| [Value](../../aspose.cells.slicers/slicercacheitem/value/) { get; } | Возвращает текст метки для элемента slicer. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerCacheItemDemo
    {
        public static void Run()
        {
            // Загрузить книгу с slicer
            Workbook workbook = new Workbook("example.xlsx");
            workbook.Worksheets.RefreshAll();

            // Получить первый slicer в книге
            var slicer = workbook.Worksheets
                .SelectMany(x => x.Slicers)
                .First();

            // Перебрать элементы кэша slicer
            Console.WriteLine("Slicer Cache Items:");
            for (int i = 0; i < slicer.SlicerCache.SlicerCacheItems.Count; i++)
            {
                SlicerCacheItem slicerCacheItem = slicer.SlicerCache.SlicerCacheItems[i];
                Console.WriteLine($"Item {i}: Selected={slicerCacheItem.Selected}, Value={slicerCacheItem.Value}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


