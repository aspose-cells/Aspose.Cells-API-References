---
title: "PivotTable.ShowDrill"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Получает и задаёт, отображаются ли кнопки раскрытия/сворачивания"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showdrill/
---
## PivotTable.ShowDrill property

Получает и задаёт, показывать ли кнопки раскрытия/сворачивания.

```csharp
public bool ShowDrill { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowDrillDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте лист и заполните его образцовыми данными
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Name = "Pivot";
            sheet.Cells["A1"].Value = "Category";
            sheet.Cells["B1"].Value = "Value";
            sheet.Cells["A2"].Value = "A";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["A3"].Value = "B";
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["A4"].Value = "A";
            sheet.Cells["B4"].Value = 150;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Настройте сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Включить детализацию и показывать индикаторы drill
            pivotTable.EnableDrilldown = true;
            pivotTable.ShowDrill = true;
            
            // Обновить и вычислить данные
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotTableShowDrillDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


