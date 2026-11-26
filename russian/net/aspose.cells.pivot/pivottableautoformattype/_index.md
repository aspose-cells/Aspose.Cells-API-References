---
title: "Перечисление PivotTableAutoFormatType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Pivot.PivotTableAutoFormatType. Представляет тип автоматического формата PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivottableautoformattype/
---
## PivotTableAutoFormatType enumeration

Представляет тип автоматического форматирования сводной таблицы.

```csharp
public enum PivotTableAutoFormatType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Представляет тип формата None. |
| Classic | `1` | Представляет тип автоматического формата Classic. |
| Report1 | `2` | Представляет тип формата Report1. |
| Report2 | `3` | Представляет тип формата Report2. |
| Report3 | `4` | Представляет тип формата Report3. |
| Report4 | `5` | Представляет тип формата Report4. |
| Report5 | `6` | Представляет тип формата Report5. |
| Report6 | `7` | Представляет тип формата Report6. |
| Report7 | `8` | Представляет тип формата Report7. |
| Report8 | `9` | Представляет тип формата Report8. |
| Report9 | `10` | Представляет тип формата Report9. |
| Report10 | `11` | Представляет тип формата Report10. |
| Table1 | `12` | Представляет тип формата Table1. |
| Table2 | `13` | Представляет тип формата Table2. |
| Table3 | `14` | Представляет тип формата Table3. |
| Table4 | `15` | Представляет тип формата Table4. |
| Table5 | `16` | Представляет тип формата Table5. |
| Table6 | `17` | Представляет тип формата Table6. |
| Table7 | `18` | Представляет тип формата Table7. |
| Table8 | `19` | Представляет тип формата Table8. |
| Table9 | `20` | Представляет тип формата Table9. |
| Table10 | `21` | Представляет тип формата Table10. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableAutoFormatTypeDemo
    {
        public static void PivotTableAutoFormatTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые примерные данные для PivotTable
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

            // Добавить сводную таблицу в лист
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Установите тип автоматического формата для PivotTable
            pivotTable.AutoFormatType = PivotTableAutoFormatType.Report1;

            // Сохраните книгу
            workbook.Save("PivotTableAutoFormatTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


