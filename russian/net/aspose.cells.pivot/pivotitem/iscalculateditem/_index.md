---
title: "PivotItem.IsCalculatedItem"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotItem. Указывает, является ли этот элемент сводной таблицы вычисляемым формульным элементом"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitem/iscalculateditem/
---
## PivotItem.IsCalculatedItem property

Указывает, является ли этот элемент сводки вычисляемым элементом формулы.

```csharp
public bool IsCalculatedItem { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsCalculatedItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;
            worksheet.Cells["B5"].Value = 15;

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Вычислить данные сводной таблицы
            pivotTable.CalculateData();

            // Получить первый элемент сводной таблицы из первого поля сводной таблицы
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // Отобразить значение свойства IsCalculatedItem
            Console.WriteLine("IsCalculatedItem value: " + pivotItem.IsCalculatedItem);

            // Проверить, является ли элемент сводной таблицы вычисляемым элементом
            if (pivotItem.IsCalculatedItem)
            {
                Console.WriteLine("This pivot item is a calculated formula item.");
                Console.WriteLine("Formula: " + pivotItem.GetFormula());
            }
            else
            {
                Console.WriteLine("This pivot item is not a calculated formula item.");
            }

            // Сохраните книгу
            workbook.Save("PivotItemPropertyIsCalculatedItemDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


