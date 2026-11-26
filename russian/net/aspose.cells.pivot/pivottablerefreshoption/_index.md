---
title: "Класс PivotTableRefreshOption"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotTableRefreshOption. Представляет параметры обновления источника данных сводной таблицы."
type: docs
url: /ru/net/aspose.cells.pivot/pivottablerefreshoption/
---
## PivotTableRefreshOption class

Представляет параметры обновления источника данных сводной таблицы.

```csharp
public class PivotTableRefreshOption
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PivotTableRefreshOption](pivottablerefreshoption/)() | Представляет параметры обновления источника данных сводной таблицы. |

## Свойства

| Имя | Описание |
| --- | --- |
| [IsKeepOriginalOrder](../../aspose.cells.pivot/pivottablerefreshoption/iskeeporiginalorder/) { get; set; } | Указывает, следует ли сохранять исходный порядок элементов сводной таблицы как в старом источнике данных. |
| [KeepCachedLocalGroupData](../../aspose.cells.pivot/pivottablerefreshoption/keepcachedlocalgroupdata/) { get; set; } | Указывает, следует ли сохранять кэшированные локальные данные групп, если максимальные и минимальные значения не изменились. Значение по умолчанию — false, что означает обновление группы с локальными настройками. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablerefreshoption/reservemissingpivotitemtype/) { get; set; } | Представляет способ резервирования отсутствующих элементов сводной таблицы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableRefreshOptionDemo
    {
        public static void PivotTableRefreshOptionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Добавьте сводную таблицу на лист.
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Создать экземпляр PivotTableRefreshOption
            PivotTableRefreshOption refreshOption = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Обновить сводную таблицу с указанными параметрами
            pivotTable.RefreshData(refreshOption);
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotTableRefreshOptionExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


