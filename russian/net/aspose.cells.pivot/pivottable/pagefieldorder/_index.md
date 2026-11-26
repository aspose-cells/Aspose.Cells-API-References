---
title: "PivotTable.PageFieldOrder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Получает и задаёт порядок, в котором поля страниц добавляются в макет отчётов PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/pagefieldorder/
---
## PivotTable.PageFieldOrder property

Получает и задаёт порядок, в котором поля страниц добавляются в макет отчёта сводной таблицы.

```csharp
public PrintOrderType PageFieldOrder { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPageFieldOrderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            var cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Region";
            cells["D1"].Value = "Sales";
            
            // Добавить строки примерных данных
            for (int i = 2; i <= 10; i++)
            {
                cells[$"A{i}"].Value = $"Category{(i % 3) + 1}";
                cells[$"B{i}"].Value = $"Product{(i % 4) + 1}";
                cells[$"C{i}"].Value = $"Region{(i % 2) + 1}";
                cells[$"D{i}"].Value = i * 100;
            }

            // Создать сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:D11", "F5", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Добавить поля в области
            pivotTable.AddFieldToArea(PivotFieldType.Page, pivotTable.BaseFields["Category"]);
            pivotTable.AddFieldToArea(PivotFieldType.Page, pivotTable.BaseFields["Region"]);
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields["Product"]);
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields["Sales"]);

            // Установить порядок полей страниц и количество переносов
            pivotTable.PageFieldOrder = PrintOrderType.DownThenOver;
            pivotTable.PageFieldWrapCount = 2;

            // Сохраните книгу
            workbook.Save("PivotTablePageFieldOrderDemo_out.xlsx");
        }
    }
}
```

### См. также

* enum [PrintOrderType](../../../aspose.cells/printordertype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


