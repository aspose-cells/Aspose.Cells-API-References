---
title: "PivotFilter.FilterType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotFilter. Получает тип фильтра сводного фильтра"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfilter/filtertype/
---
## PivotFilter.FilterType property

Получает тип фильтра сводного фильтра.

```csharp
public PivotFilterType FilterType { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyFilterTypeDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("example.xlsx");
            
            // Доступ к первому листу и сводной таблице
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Применить фильтр значений (меньше 2) к первому базовому полю
            pivotTable.BaseFields[0].FilterByValue(0, PivotFilterType.ValueLessThan, 2, 0);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Перезагрузить книгу, чтобы проверить фильтр
            Workbook verifyWorkbook = new Workbook("output.xlsx");
            PivotTable verifyPivotTable = verifyWorkbook.Worksheets[0].PivotTables[0];
            
            // Получить применённый фильтр и продемонстрировать свойство FilterType
            PivotFilter filter = verifyPivotTable.BaseFields[0].GetFilters()[0];
            Console.WriteLine("Filter Type: " + filter.FilterType); // Should output ValueLessThan
            Console.WriteLine("Filter Value: " + filter.GetNumberValues()[0]); // Should output 2
        }
    }
}
```

### См. также

* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


