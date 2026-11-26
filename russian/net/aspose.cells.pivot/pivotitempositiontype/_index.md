---
title: "Перечисление PivotItemPositionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Pivot.PivotItemPositionType перечисление. Представляет тип позиции базового элемента сводки в базовом поле, когда используется расчёт ShowDataAs"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitempositiontype/
---
## PivotItemPositionType enumeration

Представляет тип позиции базового элемента сводной таблицы в базовом поле, когда используется вычисление ShowDataAs.

```csharp
public enum PivotItemPositionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Previous | `0` | Представляет предыдущий элемент сводки в PivotField. |
| Next | `1` | Представляет следующий элемент сводки в PivotField. |
| Custom | `2` | Отображает значения в разных форматах в зависимости от индекса элемента сводки в PivotField. |

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotItemPositionTypeDemo
    {
        public static void PivotItemPositionTypeExample()
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

            // Добавьте сводную таблицу на лист.
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value

            // Установите формат отображения данных, чтобы показывать значения как разницу с предыдущим элементом
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, 0, PivotItemPositionType.Previous, 0);

            // Обновить и вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotItemPositionTypeExample.xlsx");

            Console.WriteLine("Pivot table created and saved successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


