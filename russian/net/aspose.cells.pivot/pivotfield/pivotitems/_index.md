---
title: "PivotField.PivotItems"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Получает элементы сводки данного поля."
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/pivotitems/
---
## PivotField.PivotItems property

Получает элементы сводного поля.

```csharp
public PivotItemCollection PivotItems { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyPivotItemsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["A4"].Value = "A";
            worksheet.Cells["B4"].Value = 30;
            
            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Обновите данные
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Получите поле сводки и продемонстрируйте PivotItems
            PivotField field = pivotTable.RowFields[0];
            Console.WriteLine("Field Name: " + field.Name);
            Console.WriteLine("Total PivotItems: " + field.PivotItems.Count);
            
            // Отобразить все имена элементов сводки
            foreach (PivotItem item in field.PivotItems)
            {
                Console.WriteLine("Item Name: " + item.Name);
            }
        }
    }
}
```

### См. также

* class [PivotItemCollection](../../pivotitemcollection/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


