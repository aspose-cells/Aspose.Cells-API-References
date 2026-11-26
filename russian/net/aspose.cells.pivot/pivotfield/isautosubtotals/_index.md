---
title: "PivotField.IsAutoSubtotals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает, отображает ли указанный поле автоматические подытоги. По умолчанию — true."
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/isautosubtotals/
---
## PivotField.IsAutoSubtotals property

Указывает, отображает ли указанное поле автоматические промежуточные итоги. По умолчанию — true.

```csharp
public bool IsAutoSubtotals { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAutoSubtotalsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["A3"].Value = "Bikes";
            worksheet.Cells["A4"].Value = "Cars";
            worksheet.Cells["A5"].Value = "Cars";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            worksheet.Cells["B5"].Value = 4000;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поле в область строк и установите IsAutoSubtotals в false
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.IsAutoSubtotals = false; // Disable automatic subtotals

            // Добавьте поле в область данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Вычислить данные
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotFieldIsAutoSubtotalsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


