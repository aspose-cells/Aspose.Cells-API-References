---
title: "Перечисление ReserveMissingPivotItemType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Pivot.ReserveMissingPivotItemType. Представляет способ сохранения отсутствующих элементов сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/reservemissingpivotitemtype/
---
## ReserveMissingPivotItemType enumeration

Представляет способ сохранения отсутствующих элементов сводной таблицы.

```csharp
public enum ReserveMissingPivotItemType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Default | `0` | Удаляет старые отсутствующие элементы сводной таблицы и сохраняет удалённые элементы нового источника данных как отсутствующие элементы. |
| All | `1` | Сохраняет все отсутствующие элементы. |
| None | `2` | Удаляет все отсутствующие элементы сводной таблицы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class ReserveMissingPivotItemTypeDemo
    {
        public static void ReserveMissingPivotItemTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить сводную таблицу в лист
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Установить параметр ReserveMissingPivotItemType
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Вычислить сводную таблицу с указанными параметрами
            pivotTable.CalculateData(calculateOption);

            // Обновить сводную таблицу
            pivotTable.RefreshData();

            // Сохраните книгу
            workbook.Save("ReserveMissingPivotItemTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


