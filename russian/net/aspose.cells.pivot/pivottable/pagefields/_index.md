---
title: "PivotTable.PageFields"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает PivotFieldCollection, которые в настоящее время отображаются как поля страниц"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/pagefields/
---
## PivotTable.PageFields property

Возвращает [`PivotFieldCollection`](../../pivotfieldcollection/), которые в настоящее время отображаются как поля страниц.

```csharp
public PivotFieldCollection PageFields { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPageFieldsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            var cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            
            cells["A4"].Value = "P3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;
            
            cells["A5"].Value = "P1";
            cells["B5"].Value = "West";
            cells["C5"].Value = 4000;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Добавить поля
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Region");

            // Доступ к полям страниц
            PivotFieldCollection pageFields = pivotTable.PageFields;
            
            Console.WriteLine("Page Fields:");
            foreach (PivotField field in pageFields)
            {
                Console.WriteLine($"Field: {field.Name}");
                Console.WriteLine("Items:");
                foreach (PivotItem item in field.PivotItems)
                {
                    Console.WriteLine($"- {item.Name} (Hidden: {item.IsHidden})");
                }
            }

            // Сохраните книгу
            workbook.Save("PivotTablePageFieldsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


