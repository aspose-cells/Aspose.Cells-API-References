---
title: "Перечисление PivotFieldType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Pivot.PivotFieldType. Представляет тип поля PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldtype/
---
## PivotFieldType enumeration

Представляет тип поля PivotTable.

```csharp
public enum PivotFieldType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `0` | Представляет базовый тип поля сводной таблицы. |
| Row | `1` | Представляет тип поля строки сводной таблицы. |
| Column | `2` | Представляет тип поля столбца сводной таблицы. |
| Page | `4` | Представляет тип поля страницы сводной таблицы. |
| Data | `8` | Представляет тип поля данных сводной таблицы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldTypeDemo
    {
        public static void PivotFieldTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Grape";
            worksheet.Cells[2, 0].Value = "Blueberry";
            worksheet.Cells[3, 0].Value = "Kiwi";
            worksheet.Cells[4, 0].Value = "Cherry";
            worksheet.Cells[5, 0].Value = "Grape";
            worksheet.Cells[6, 0].Value = "Blueberry";
            worksheet.Cells[7, 0].Value = "Kiwi";
            worksheet.Cells[8, 0].Value = "Cherry";

            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[4, 1].Value = 2020;
            worksheet.Cells[5, 1].Value = 2021;
            worksheet.Cells[6, 1].Value = 2021;
            worksheet.Cells[7, 1].Value = 2021;
            worksheet.Cells[8, 1].Value = 2021;

            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 2].Value = 80;
            worksheet.Cells[5, 2].Value = 90;
            worksheet.Cells[6, 2].Value = 100;
            worksheet.Cells[7, 2].Value = 110;
            worksheet.Cells[8, 2].Value = 120;

            // Добавить сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "A12", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Установить стиль pivot table
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium9;

            // Обновить и вычислить данные
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotFieldTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


