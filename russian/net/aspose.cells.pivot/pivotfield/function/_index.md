---
title: "PivotField.Function"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Представляет функцию, используемую для суммирования этого поля данных PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/function/
---
## PivotField.Function property

Представляет функцию, используемую для суммирования этого поля данных сводной таблицы.

```csharp
public ConsolidationFunction Function { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyFunctionDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте примерные данные
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "A";
            cells["B2"].Value = 100;
            cells["A3"].Value = "B";
            cells["B3"].Value = 120;
            cells["A4"].Value = "A";
            cells["B4"].Value = 80;
            cells["A5"].Value = "B";
            cells["B5"].Value = 60;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Добавьте поле данных и установите функцию в Max
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[fieldIndex];
            dataField.Function = ConsolidationFunction.Max;

            // Вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotFieldFunctionDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


