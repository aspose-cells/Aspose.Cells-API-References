---
title: "PivotItem.IsDetailHidden"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotItem. Получает и задаёт, скрыты ли детали этого элемента сводки"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitem/isdetailhidden/
---
## PivotItem.IsDetailHidden property

Получает и задает, скрыты ли детали этого элемента сводки.

```csharp
public bool IsDetailHidden { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIsDetailHiddenDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Fruit");
            sheet.Cells["A4"].PutValue("Vegetable");
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Item");
            sheet.Cells["B2"].PutValue("Apple");
            sheet.Cells["B3"].PutValue("Orange");
            sheet.Cells["B4"].PutValue("Carrot");
            sheet.Cells["B5"].PutValue("Potato");
            sheet.Cells["C1"].PutValue("Amount");
            sheet.Cells["C2"].PutValue(10);
            sheet.Cells["C3"].PutValue(15);
            sheet.Cells["C4"].PutValue(20);
            sheet.Cells["C5"].PutValue(25);

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Добавить поля строк
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            
            // Обновить и вычислить данные
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Скрыть детали категории "Fruit"
            pivotTable.RowFields[0].PivotItems["Fruit"].IsDetailHidden = true;
            
            // Сохраните книгу
            wb.Save("PivotItemIsDetailHiddenDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


