---
title: "PivotFilterCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotFilterCollection. Добавляет объект PivotFilter к конкретному типу"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfiltercollection/add/
---
## PivotFilterCollection.Add method

Добавляет объект PivotFilter к конкретному типу

```csharp
[Obsolete("Use PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() and AddDateFilter() methods,instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int fieldIndex, PivotFilterType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | Int32 | индекс PivotField |
| type | PivotFilterType | тип PivotFilter |

### Возвращаемое значение

индекс объекта PivotFilter в этой PivotFilterCollection.

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте методы PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() и AddDateFilter(). Этот метод будет удалён через 12 месяцев, начиная с ноября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterCollectionMethodAddWithInt32PivotFilterTypeDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Пример данных
            cells["A1"].Value = "Category";
            cells["A2"].Value = "A";
            cells["A3"].Value = "B";
            cells["A4"].Value = "A";
            cells["A5"].Value = "B";
            
            cells["B1"].Value = "Value";
            cells["B2"].Value = 10;
            cells["B3"].Value = 20;
            cells["B4"].Value = 30;
            cells["B5"].Value = 40;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Value");

            // Добавить фильтр сводной таблицы
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            pivot.RefreshData();
            pivot.CalculateData();

            book.Save("PivotFilterDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


