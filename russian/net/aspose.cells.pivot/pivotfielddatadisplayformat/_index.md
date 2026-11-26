---
title: "Перечисление PivotFieldDataDisplayFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Pivot.PivotFieldDataDisplayFormat. Представляет формат отображения данных в поле данных сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfielddatadisplayformat/
---
## PivotFieldDataDisplayFormat enumeration

Представляет формат отображения данных в поле данных сводной таблицы.

```csharp
public enum PivotFieldDataDisplayFormat
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Normal | `0` | Представляет обычный формат отображения. |
| DifferenceFrom | `1` | Представляет формат отображения разницы. |
| PercentageOf | `2` | Представляет процентный формат отображения. |
| PercentageDifferenceFrom | `3` | Представляет процентную разницу формата отображения. |
| RunningTotalIn | `4` | Представляет накопительный итог в формате отображения. |
| PercentageOfRow | `5` | Представляет процентный формат отображения строки. |
| PercentageOfColumn | `6` | Представляет процентный формат отображения столбца. |
| PercentageOfTotal | `7` | Представляет процентный формат общего отображения. |
| Index | `8` | Представляет формат отображения индекса. |
| PercentageOfParentRowTotal | `9` | Представляет процентный формат общего отображения родительской строки. |
| PercentageOfParentColumnTotal | `10` | Представляет процентный формат общего отображения родительского столбца. |
| PercentageOfParentTotal | `11` | Представляет процентный формат общего отображения родительского итога. |
| PercentageOfRunningTotalIn | `12` | Представляет процентный формат накопительного итога в отображении. |
| RankSmallestToLargest | `13` | Представляет формат отображения от наименьшего к наибольшему. |
| RankLargestToSmallest | `14` | Представляет формат отображения от наибольшего к наименьшему. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldDataDisplayFormatDemo
    {
        public static void PivotFieldDataDisplayFormatExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Добавьте некоторые образцы данных.
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Добавить сводную таблицу
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Установите стиль сводной таблицы
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Изменить атрибуты PivotField
            PivotField dataField = pivot.DataFields[0];
            dataField.DisplayName = "custom display name";

            // Установить DataDisplayFormat
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;

            // Обновить и вычислить данные
            pivot.RefreshData();
            pivot.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotFieldDataDisplayFormatExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


