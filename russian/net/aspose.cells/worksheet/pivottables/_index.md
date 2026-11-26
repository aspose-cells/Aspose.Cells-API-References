---
title: "Worksheet.PivotTables"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает все сводные таблицы в этом листе"
type: docs
url: /ru/net/aspose.cells/worksheet/pivottables/
---
## Worksheet.PivotTables property

Получает все сводные таблицы в этом листе.

```csharp
public PivotTableCollection PivotTables { get; }
```

### Примеры

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPivotTablesDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("PivotTableExample.xlsx");
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к коллекции сводных таблиц листа
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Проверьте, есть ли сводные таблицы
            if (pivotTables.Count > 0)
            {
                // Получить первую сводную таблицу
                PivotTable pivotTable = pivotTables[0];
                
                // Очистить все существующие фильтры
                pivotTable.PivotFilters.Clear();
                
                // Обновить данные сводной таблицы
                pivotTable.RefreshData();
                pivotTable.CalculateData();
                
                // Сохранить изменённую книгу
                workbook.Save("PivotTableModified.xlsx");
            }
        }
    }
}
```

### См. также

* class [PivotTableCollection](../../../aspose.cells.pivot/pivottablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


