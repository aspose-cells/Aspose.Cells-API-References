---
title: "PivotField.DisplayName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Представляет отображаемое имя поля сводной таблицы в представлении сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/displayname/
---
## PivotField.DisplayName property

Представляет отображаемое имя поля сводной таблицы в представлении сводной таблицы.

```csharp
public string DisplayName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDisplayNameDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу и добавьте примерные данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить поле строки и поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Установите пользовательское отображаемое имя для поля данных
            pivotTable.DataFields[0].DisplayName = "Total Sales";
            
            // Обновить и вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Получить доступ к ячейке, используя отображаемое имя
            Cell cell = pivotTable.GetCellByDisplayName("Total Sales");
            Console.WriteLine("Cell found at row: {0}, column: {1}", cell.Row, cell.Column);
            
            // Сохраните книгу
            workbook.Save("PivotFieldDisplayNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


