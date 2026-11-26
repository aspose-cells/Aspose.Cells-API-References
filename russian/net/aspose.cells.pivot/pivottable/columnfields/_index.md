---
title: "PivotTable.ColumnFields"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает объект PivotFields, который в данный момент отображается как столбцовые поля"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/columnfields/
---
## PivotTable.ColumnFields property

Возвращает объект PivotFields, который в данный момент отображается как столбцовые поля.

```csharp
public PivotFieldCollection ColumnFields { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyColumnFieldsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            var cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bikes";
            cells["B2"].Value = 100;
            cells["A3"].Value = "Bikes";
            cells["B3"].Value = 200;
            cells["A4"].Value = "Cars";
            cells["B4"].Value = 300;
            cells["A5"].Value = "Cars";
            cells["B5"].Value = 400;
            cells["A6"].Value = "Trucks";
            cells["B6"].Value = 500;

            // Добавьте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поля строк и столбцов
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Sales");

            // Получите доступ и измените столбцовое поле
            PivotField columnField = pivotTable.ColumnFields[0];
            columnField.FilterByValue(0, PivotFilterType.ValueGreaterThan, 300, 0);

            // Вычислите и обновите данные
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotTableColumnFieldsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


