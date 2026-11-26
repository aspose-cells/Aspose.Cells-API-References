---
title: "PivotTable.AllowMultipleFiltersPerField"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает логическое значение, определяющее, могут ли поля PivotTable иметь несколько фильтров, установленных для них"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/allowmultiplefiltersperfield/
---
## PivotTable.AllowMultipleFiltersPerField property

Указывает логическое значение, которое определяет, могут ли поля PivotTable иметь несколько установленных фильтров.

```csharp
public bool AllowMultipleFiltersPerField { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAllowMultipleFiltersPerFieldDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 10;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Установить свойство AllowMultipleFiltersPerField
            pivotTable.AllowMultipleFiltersPerField = true;
            Console.WriteLine("AllowMultipleFiltersPerField: " + pivotTable.AllowMultipleFiltersPerField);

            // Сохраните книгу
            workbook.Save("PivotTable_AllowMultipleFiltersPerField.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


