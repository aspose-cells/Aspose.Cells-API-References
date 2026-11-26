---
title: "Перечисление PivotFieldSubtotalType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Pivot.PivotFieldSubtotalType перечисление. Краткое описание PivotFieldSubtotalType"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldsubtotaltype/
---
## PivotFieldSubtotalType enumeration

Краткое описание для PivotFieldSubtotalType.

```csharp
[Flags]
public enum PivotFieldSubtotalType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Представляет тип подытога None. |
| Automatic | `1` | Представляет тип подытога Automatic. |
| Sum | `2` | Представляет тип подытога Sum. |
| Count | `4` | Представляет тип подытога Count. |
| Average | `8` | Представляет тип подытога Average. |
| Max | `10` | Представляет тип подытога Max. |
| Min | `20` | Представляет тип подытога Min. |
| Product | `40` | Представляет тип подытога Product. |
| CountNums | `80` | Представляет тип подытога Count Nums. |
| Stdev | `100` | Представляет тип подытога стандартного отклонения. |
| Stdevp | `200` | Представляет тип подытога стандартного отклонения популяции. |
| Var | `400` | Представляет тип подытога дисперсии. |
| Varp | `800` | Представляет тип подытога дисперсии популяции. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSubtotalTypeDemo
    {
        public static void PivotFieldSubtotalTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Добавить сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Установить тип подытога для поля строки
            PivotField rowField = pivotTable.RowFields[0];
            rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            rowField.SetSubtotals(PivotFieldSubtotalType.Count, true);

            // Обновить и вычислить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotFieldSubtotalTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


