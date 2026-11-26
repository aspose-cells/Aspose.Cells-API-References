---
title: "PivotItem.IsHidden"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotItem. Получает и задает, скрыт ли элемент сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitem/ishidden/
---
## PivotItem.IsHidden property

Получает и задает, скрыт ли элемент сводки.

```csharp
public bool IsHidden { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "债券借贷";
            worksheet.Cells["A3"].Value = "股票";
            worksheet.Cells["A4"].Value = "基金";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Получить доступ к полю сводной таблицы и элементам
            PivotField field = pivotTable.RowFields[0];
            
            // Установить свойство IsHidden, чтобы показывать только "债券借贷"
            foreach (PivotItem item in field.PivotItems)
            {
                item.IsHidden = (item.Name != "债券借贷");
            }

            // Обновить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotItemIsHiddenDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


