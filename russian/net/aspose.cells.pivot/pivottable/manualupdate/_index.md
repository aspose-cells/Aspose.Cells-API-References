---
title: "PivotTable.ManualUpdate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, пересчитывается ли отчет PivotTable только по запросу пользователя"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/manualupdate/
---
## PivotTable.ManualUpdate property

Указывает, пересчитывается ли отчёт сводной таблицы только по запросу пользователя.

```csharp
public bool ManualUpdate { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyManualUpdateDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Добавьте лист и заполните его образцовыми данными
            Worksheet dataSheet = workbook.Worksheets["Sheet1"];
            dataSheet.Cells["A1"].PutValue("Category");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);
            dataSheet.Cells["A4"].PutValue("A");
            dataSheet.Cells["B4"].PutValue(30);

            // Добавить сводную таблицу
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            int index = pivotSheet.PivotTables.Add("Sheet1!A1:B4", "A3", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[index];

            // Настройте сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Включить ручное обновление
            pivotTable.ManualUpdate = true;
            
            // На данный момент сводная таблица не будет обновляться автоматически
            Console.WriteLine("Pivot table before refresh (ManualUpdate=true):");
            Console.WriteLine(pivotSheet.Cells["B4"].StringValue); // Will be empty
            
            // Вручную обновить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            Console.WriteLine("Pivot table after manual refresh:");
            Console.WriteLine(pivotSheet.Cells["B4"].StringValue); // Will show "40" (sum of category A)
            
            // Сохраните книгу
            workbook.Save("PivotTableManualUpdateDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


