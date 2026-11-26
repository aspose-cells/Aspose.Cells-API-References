---
title: "PivotTable.ShowDataTips"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, следует ли отображать подсказки для ячеек данных PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showdatatips/
---
## PivotTable.ShowDataTips property

Указывает, следует ли отображать подсказки для ячеек данных PivotTable.

```csharp
public bool ShowDataTips { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowDataTipsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте лист и некоторые примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 20;

            // Создайте сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Настройте сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Включить подсказки данных
            pivotTable.ShowDataTips = true;
            
            // Сохраните книгу
            workbook.Save("PivotTableWithDataTips.xlsx");
            
            Console.WriteLine("Pivot table with ShowDataTips enabled created successfully.");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


