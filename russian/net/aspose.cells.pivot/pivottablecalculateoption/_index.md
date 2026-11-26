---
title: "Класс PivotTableCalculateOption"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotTableCalculateOption. Представляет параметры вычисления данных сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottablecalculateoption/
---
## PivotTableCalculateOption class

Представляет параметры расчёта данных сводной таблицы.

```csharp
public class PivotTableCalculateOption
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PivotTableCalculateOption](pivottablecalculateoption/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [RefreshCharts](../../aspose.cells.pivot/pivottablecalculateoption/refreshcharts/) { get; set; } | Указывает, обновляются ли диаграммы на основе этой сводной таблицы. |
| [RefreshData](../../aspose.cells.pivot/pivottablecalculateoption/refreshdata/) { get; set; } | Указывает, обновляется ли источник данных сводной таблицы. |
| [RefreshOption](../../aspose.cells.pivot/pivottablecalculateoption/refreshoption/) { get; set; } | Получает и задает параметры обновления источника данных в кэш сводной таблицы. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/) { get; set; } | Представляет способ резервирования отсутствующих элементов сводной таблицы. |

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionDemo
    {
        public static void PivotTableCalculateOptionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте некоторые данные для сводной таблицы
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Fruit");
            sheet.Cells["B4"].PutValue(70);
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B5"].PutValue(40);

            // Добавьте сводную таблицу на лист.
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Настройте сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Создайте объект PivotTableCalculateOption
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Вычислите данные сводной таблицы с указанными параметрами
            pivotTable.CalculateData(calculateOption);

            // Сохраните книгу
            workbook.Save("PivotTableCalculateOptionExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


