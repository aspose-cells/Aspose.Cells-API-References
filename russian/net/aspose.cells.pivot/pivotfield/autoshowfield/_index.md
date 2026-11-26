---
title: "PivotField.AutoShowField"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Представляет индекс поля автоотображения. 1 означает само поле PivotField. Это должен быть индекс полей данных."
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/autoshowfield/
---
## PivotField.AutoShowField property

Представляет индекс поля автоотображения. -1 означает само поле PivotField. Это должен быть индекс полей данных.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.RankBy property or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoShowField { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.Top10AutoShowSettings.RankBy или метод PivotField.Top10AutoShow(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoShowFieldDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook();
            
            // Добавьте лист и заполните его образцовыми данными
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Добавить примерные данные для сводной таблицы
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
            
            // Добавить поле строки и поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Настроить AutoShow для первого поля сводки
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.AutoShowCount = 2;
            pivotField.AutoShowField = 1; // Index of data field (Quantity)
            pivotField.IsAutoShow = true;
            pivotField.IsAscendShow = true; // Equivalent to "Top" in AutoShowType
            
            // Сохраните книгу
            workbook.Save("PivotField_AutoShowField_Example.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


