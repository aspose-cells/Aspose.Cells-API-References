---
title: "PivotTable.PageFieldWrapCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает количество полей страниц в каждом столбце или строке отчёта PivotTable."
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/pagefieldwrapcount/
---
## PivotTable.PageFieldWrapCount property

Получает количество полей страниц в каждом столбце или строке отчёта сводной таблицы.

```csharp
public int PageFieldWrapCount { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPageFieldWrapCountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Вставить данные
            Worksheet data = workbook.Worksheets.Add("data");
            data.Cells["A1"].PutValue("Country");
            data.Cells["B1"].PutValue("Product");
            data.Cells["C1"].PutValue("Vendor");
            data.Cells["D1"].PutValue("Value");
            data.Cells["A2"].PutValue("USA");
            data.Cells["B2"].PutValue("Car");
            data.Cells["C2"].PutValue("Ford");
            data.Cells["D2"].PutValue(1200.987654321);
            data.Cells["A3"].PutValue("Japan");
            data.Cells["B3"].PutValue("Bike");
            data.Cells["C3"].PutValue("Yamaha");
            data.Cells["D3"].PutValue(985.123456789);

            // Создать сводную таблицу
            Worksheet pivot = workbook.Worksheets.Add("pivot");
            PivotTableCollection pivotTables = pivot.PivotTables;
            int index = pivotTables.Add("=data!A1:D3", "A1", "pivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Vendor");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Установить свойство PageFieldWrapCount
            pivotTable.PageFieldWrapCount = 2; // Number of page fields per row
            
            // Вычислить и обновить сводную таблицу
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotTablePageFieldWrapCountDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


