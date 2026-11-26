---
title: "PivotArea.PivotArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор PivotArea. Представляет выбранную область PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivotarea/pivotarea/
---
## PivotArea constructor

Представляет выбранную область сводной таблицы.

```csharp
public PivotArea(PivotTable table)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| таблица | PivotTable |  |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodctorWithPivotTableDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Продемонстрировать конструктор PivotArea с параметром PivotTable
            PivotArea pivotArea = new PivotArea(pivotTable);
            
            // Настроить область сводной таблицы
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            
            // Сохраните книгу
            workbook.Save("PivotAreaDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../../pivottable/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


