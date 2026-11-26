---
title: "PivotTable.BaseFields"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает все базовые поля сводной таблицы в PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/basefields/
---
## PivotTable.BaseFields property

Возвращает все базовые поля сводной таблицы в PivotTable.

```csharp
public PivotFieldCollection BaseFields { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyBaseFieldsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 5;

            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Обновить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Получить доступ к коллекции BaseFields
            PivotFieldCollection baseFields = pivotTable.BaseFields;
            
            // Отобразить оригинальные элементы из каждого базового поля
            Console.WriteLine("Base Fields and their Original Items:");
            foreach (PivotField field in baseFields)
            {
                Console.WriteLine($"Field: {field.Name}");
                string[] originalItems = field.OriginalItems;
                foreach (string item in originalItems)
                {
                    Console.WriteLine($"- {item}");
                }
            }
        }
    }
}
```

### См. также

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


