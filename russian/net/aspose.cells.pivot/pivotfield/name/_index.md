---
title: "PivotField.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Представляет имя PivotField"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/name/
---
## PivotField.Name property

Представляет имя PivotField.

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
    public class PivotFieldPropertyNameDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = new DateTime(2024, 1, 5);
            sheet.Cells["A3"].Value = new DateTime(2024, 1, 10);
            sheet.Cells["A4"].Value = new DateTime(2024, 2, 15);
            sheet.Cells["A5"].Value = new DateTime(2024, 3, 20);
            
            sheet.Cells["B1"].Value = "Value";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["B4"].Value = 300;
            sheet.Cells["B5"].Value = 400;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pt = sheet.PivotTables[index];
            
            // Добавьте поле строки и продемонстрируйте свойство Name
            pt.AddFieldToArea(PivotFieldType.Row, 0);
            pt.RowFields[0].Name = "MyDateField";
            
            // Группировать по месяцам и годам
            DateTime start = new DateTime(2024, 1, 1);
            DateTime end = new DateTime(2024, 12, 31);
            pt.RowFields[0].GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, true);
            
            // Выведите имена сгруппированных полей
            Console.WriteLine("Row Field 0 Name: " + pt.RowFields[0].Name); // Will show "MyYears"
            Console.WriteLine("Row Field 1 Name: " + pt.RowFields[1].Name); // Will show "MyMonths"
            
            // Сохраните книгу
            wb.Save("PivotFieldNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


