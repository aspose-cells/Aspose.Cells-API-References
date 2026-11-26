---
title: "PivotField.Number"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Представляет встроенный формат отображения чисел и дат"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/number/
---
## PivotField.Number property

Представляет встроенный формат отображения чисел и дат.

```csharp
public int Number { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNumberDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(new DateTime(2023, 1, 8));
            sheet.Cells["A3"].PutValue(new DateTime(2023, 1, 15));
            sheet.Cells["A4"].PutValue(new DateTime(2023, 1, 22));
            
            // Создать сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // Добавить поле даты в область столбцов и установить числовой формат
            int fieldIndex = pivot.AddFieldToArea(PivotFieldType.Column, 0);
            PivotField field = pivot.ColumnFields[fieldIndex];
            field.Number = 16; // d-mmm format
            
            // Обновить и вычислить сводную таблицу
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotFieldNumberDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


