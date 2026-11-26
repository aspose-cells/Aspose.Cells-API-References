---
title: "PivotItem.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotItem. Получает имя элемента сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitem/name/
---
## PivotItem.Name property

Получает имя элемента сводки.

```csharp
public string Name { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyNameDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            ws.Cells["A1"].Value = "Category";
            ws.Cells["B1"].Value = "Value";
            ws.Cells["A2"].Value = "债券借贷";
            ws.Cells["A3"].Value = "股票";
            ws.Cells["A4"].Value = "基金";
            ws.Cells["B2"].Value = 100;
            ws.Cells["B3"].Value = 200;
            ws.Cells["B4"].Value = 300;

            // Создать сводную таблицу
            int index = ws.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = ws.PivotTables[index];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Получите доступ к элементам сводной таблицы и продемонстрируйте свойство Name
            PivotField field = pivotTable.RowFields[0];
            foreach (PivotItem item in field.PivotItems)
            {
                // Скрыть все элементы, кроме "债券借贷"
                item.IsHidden = item.Name != "债券借贷";
                Console.WriteLine($"Pivot Item Name: {item.Name}, Hidden: {item.IsHidden}");
            }
            
            // Обновить и сохранить
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            wb.Save("PivotItemNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


