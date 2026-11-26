---
title: "PivotTable.ErrorString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает строку, отображаемую в ячейках, содержащих ошибки, когда свойство DisplayErrorString установлено в true. Значение по умолчанию — пустая строка."
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/errorstring/
---
## PivotTable.ErrorString property

Получает строку, отображаемую в ячейках, содержащих ошибки, когда свойство DisplayErrorString равно true. Значение по умолчанию — пустая строка.

```csharp
public string ErrorString { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyErrorStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 1800;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Установить свойство ErrorString
            pivotTable.ErrorString = "Custom Error";
            pivotTable.DisplayErrorString = true;

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Вычислите данные и обновите сводную таблицу
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Сохраните книгу
            workbook.Save("PivotTableErrorStringDemo.xlsx");

            Console.WriteLine("PivotTable with ErrorString property set successfully.");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


