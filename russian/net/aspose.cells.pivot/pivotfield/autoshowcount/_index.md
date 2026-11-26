---
title: "PivotField.AutoShowCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Представляет количество верхних или нижних элементов, которые автоматически отображаются в указанном поле сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/autoshowcount/
---
## PivotField.AutoShowCount property

Представляет количество верхних или нижних элементов, автоматически отображаемых в указанном поле PivotTable.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.AutoShowCount property or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoShowCount { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.Top10AutoShowSettings.AutoShowCount или метод PivotField.Top10AutoShow(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoShowCountDemo
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
            cells["B6"].Value = 25;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Добавьте поле строки и установите свойства AutoShow
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            rowField.AutoShowCount = 2;
            rowField.IsAutoShow = true;
            rowField.AutoShowField = 1; // Index of "Quantity" field (0-based)

            // Вычислите данные и сохраните
            pivotTable.CalculateData();
            workbook.Save("PivotFieldAutoShowCountDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


