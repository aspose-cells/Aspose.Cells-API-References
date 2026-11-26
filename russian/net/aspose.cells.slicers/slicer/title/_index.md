---
title: "Slicer.Title"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Slicer property. Указывает заголовок текущего объекта Slicer"
type: docs
url: /ru/net/aspose.cells.slicers/slicer/title/
---
## Slicer.Title property

Указывает заголовок текущего объекта Slicer.

```csharp
[Obsolete("Use Shape.Title property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string Title { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [`Title`](../../../aspose.cells.drawing/shape/title/). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyTitleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C1", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.CalculateData();

            // Добавить срез
            SlicerCollection slicers = worksheet.Slicers;
            int slicerIndex = slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = slicers[slicerIndex];
            
            // Установить заголовок среза
            slicer.Title = "Fruit Selection Slicer";
            
            // Сохраните книгу
            workbook.Save("SlicerTitleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


