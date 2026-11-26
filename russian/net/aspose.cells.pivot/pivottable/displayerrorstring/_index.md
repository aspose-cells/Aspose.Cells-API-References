---
title: "PivotTable.DisplayErrorString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, отображает ли отчёт PivotTable пользовательскую строку в ячейках, содержащих ошибки."
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/displayerrorstring/
---
## PivotTable.DisplayErrorString property

Указывает, отображает ли отчет PivotTable пользовательскую строку в ячейках, содержащих ошибки.

```csharp
public bool DisplayErrorString { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDisplayErrorStringDemo
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
            cells["B5"].Value = 2500;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Установить свойство DisplayErrorString и продемонстрировать его использование
            pivotTable.DisplayErrorString = true;
            pivotTable.ErrorString = "Custom Error";

            // Вычислить данные, чтобы показать эффект
            pivotTable.CalculateData();

            Console.WriteLine("DisplayErrorString is set to: " + pivotTable.DisplayErrorString);
            Console.WriteLine("ErrorString is set to: " + pivotTable.ErrorString);

            // Сохраните книгу
            workbook.Save("PivotTablePropertyDisplayErrorStringDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


