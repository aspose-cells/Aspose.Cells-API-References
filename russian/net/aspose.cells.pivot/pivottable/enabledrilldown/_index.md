---
title: "PivotTable.EnableDrilldown"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, включено ли углубление"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/enabledrilldown/
---
## PivotTable.EnableDrilldown property

Указывает, включено ли раскрытие (drilldown).

```csharp
public bool EnableDrilldown { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableDrilldownDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте лист и заполните его образцовыми данными
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Создайте сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Настроить поля сводной таблицы
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Включить функцию углубления
            pivotTable.EnableDrilldown = true;
            
            // Сохраните книгу
            workbook.Save("PivotTableEnableDrilldownDemo.xlsx");
            
            // Проверьте, что свойство было установлено
            Console.WriteLine("EnableDrilldown property is set to: " + pivotTable.EnableDrilldown);
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


