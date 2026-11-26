---
title: "PivotFilter.FieldIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotFilter. Получает индекс исходного поля, к которому применяется этот сводный фильтр"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfilter/fieldindex/
---
## PivotFilter.FieldIndex property

Получает индекс исходного поля, к которому применяется этот сводный фильтр.

```csharp
public int FieldIndex { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 8;

            // Добавьте сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Добавить поле строки и поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Добавить фильтр
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField pivotField = pivotTable.PageFields[0];
            
            // Создать коллекцию сводных фильтров и добавить фильтр
            PivotFilterCollection filters = pivotTable.PivotFilters;
            int filterIndex = filters.Add(0, PivotFilterType.Count);
            PivotFilter filter = filters[filterIndex];
            
            // Продемонстрировать свойство FieldIndex
            Console.WriteLine("Field Index: " + filter.FieldIndex);

            // Сохраните книгу
            workbook.Save("PivotFilterFieldIndexDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


