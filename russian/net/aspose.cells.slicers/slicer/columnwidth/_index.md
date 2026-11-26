---
title: "Slicer.ColumnWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Slicer. Возвращает или задает ширину каждого столбца в срезе в единицах точек"
type: docs
url: /ru/net/aspose.cells.slicers/slicer/columnwidth/
---
## Slicer.ColumnWidth property

Возвращает или задает ширину каждого столбца в slicer в единицах точек.

```csharp
public double ColumnWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyColumnWidthDemo
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
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            
            // Добавьте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Добавить срез
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "A1");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Установить ширину столбца в точках
            slicer.ColumnWidth = 80;
            
            // Сохраните книгу
            workbook.Save("SlicerColumnWidthDemo.xlsx");
        }
    }
}
```

### См. также

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


