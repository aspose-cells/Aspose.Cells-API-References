---
title: "PivotFilter.GetTop10Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotFilter. Получает настройку топ‑10 фильтра"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfilter/gettop10value/
---
## PivotFilter.GetTop10Value method

Получает настройку топ‑10 фильтра.

```csharp
public Top10Filter GetTop10Value()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetTop10ValueDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("example.xlsx");
            
            // Доступ к первому листу и сводной таблице
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Применить фильтр топ‑10 к первому базовому полю (показать 2 лучших элемента по количеству)
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // Получить применённый фильтр и его значение топ‑10
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            Top10Filter top10Filter = filter.GetTop10Value();
            
            // Вывести детали фильтра
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Top 10 Items: " + top10Filter.Items);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Top10Filter](../../../aspose.cells/top10filter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


