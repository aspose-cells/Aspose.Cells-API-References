---
title: "PivotTableCalculateOption.ReserveMissingPivotItemType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTableCalculateOption. Представляет способ резервирования отсутствующих элементов сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/
---
## PivotTableCalculateOption.ReserveMissingPivotItemType property

Представляет способ резервирования отсутствующих элементов сводной таблицы.

```csharp
public ReserveMissingPivotItemType ReserveMissingPivotItemType { get; set; }
```

### Примечания

Работает только когда [`RefreshData`](../refreshdata/) равно true.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyReserveMissingPivotItemTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Пример данных
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("A");
            sheet.Cells["B4"].PutValue(30);

            // Создать сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Настройте поля сводной таблицы
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Установите параметры расчёта с ReserveMissingPivotItemType
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Вычислить с параметрами
            pivotTable.CalculateData(options);

            // Сохранить результат
            workbook.Save("PivotTableReserveMissingItemsDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ReserveMissingPivotItemType](../../reservemissingpivotitemtype/)
* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


