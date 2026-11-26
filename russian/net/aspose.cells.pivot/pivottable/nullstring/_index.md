---
title: "PivotTable.NullString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает строку, отображаемую в ячейках, содержащих нулевые значения, когда свойство DisplayNullString равно true. Значение по умолчанию — пустая строка."
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/nullstring/
---
## PivotTable.NullString property

Получает строку, отображаемую в ячейках, содержащих null‑значения, когда свойство DisplayNullString равно true. Значение по умолчанию — пустая строка.

```csharp
public string NullString { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyNullStringDemo
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
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 3000;
            cells["A5"].Value = null; // Null value
            cells["B5"].Value = 4000;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Установить свойство NullString и параметры отображения
            pivotTable.NullString = "(null)";
            pivotTable.DisplayNullString = true;

            // Обновить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotTableNullStringDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


